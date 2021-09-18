package interviewjavaprogram;

import java.util.Scanner;

// prime number --- Numbers are divisible by only 1 and  itself.
// e.g  3,5,7,11,13,17,19.........

public class PrimeNumberChecker {
	
	static int number ,flag = 0;
	
	public static void prime(int number) {
		
		if(number == 0 || number == 1) {
			System.out.println(number + "is not prime ");
		}else {
			
			for (int i = 2; i < number -1; i++) {
				
				if(number % i == 0) {
					System.out.println(number + "is not prime ");
					++flag;
					break;
				}
				
			}
		}
		if (flag == 0) {
			System.out.println(number + " is a prime number");
		}
		
		
		
			
	}
	
	public static void main(String[] args) {
		Scanner user = new Scanner(System.in);
		System.out.println("Enter number ");
		number = user.nextInt();
		prime(number);
	}
		
	}
	
	
	

	



