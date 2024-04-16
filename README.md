// Booksale-Inventory-System
import java.util.*;

public class Activity8_BubbleSort {

	public static void main(String[] args) {
		
		Scanner scan = new Scanner(System.in);
		
		String[] number = new String[4];
		String temp;
		
		System.out.println("Enter Values: ");
		for(int i = 0; i < number.length; i++) {
			number[i] = scan.nextLine();
		}
		
		for(int i = 0; i < number.length; i++) {
			System.out.println(number[i] + " ");
		}
		
		System.out.println();
		for(int i = 0; i < number.length - 1; i++) {
			for(int j = 0; j < number.length - i - 1; j++) {
				if(number[j].compareTo(number[j+1]) > 0) {
					temp = number[j];
					number[j] = number[j + 1];
					number[j+1] = temp;
				}
			}
		}
		
		System.out.println();
		for(int i = 0; i < number.length; i++) {
			System.out.println(number[i] + " ");
		}

	}

}
