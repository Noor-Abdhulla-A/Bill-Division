# Bill-Division
# Hackerrank Problem Solution in java

import java.util.Scanner;

public class Billdivision {

	public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        int n = scan.nextInt();
        int k = scan.nextInt();
        int ar[] = new int [n];
        for (int i = 0; i < ar.length; i++) {
			ar[i] = scan.nextInt();
        }
        
        int sum =0;
        for (int i = 0; i < ar.length; i++) {
			
			if(i != k) {
				sum = sum + ar[i];
			}
        }
        int num = scan.nextInt();
        if(num == sum/2) {
        	System.out.println("Bon Appetit");
        }
        else {
        	System.out.println(num - sum/2);
        }
        
	}

}
