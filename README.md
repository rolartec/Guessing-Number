Guessing-Number
===============
// Guessing Number

// By  Reina Olarte

import java.util.Scanner;

						// imports the Scannner Class
import java.util.Random;
	
						//  import the random class


public class GuessingNumber
{

	public static void main(String[] args)
	
	{
		// Create the Scanner to input the number
		Scanner input = new Scanner(System.in);
		// Create the Random number
		Random randomNumber = new Random();
		
		//Declaring the variables 
		int Usernumber;
		int computerNumber;
		computerNumber = 0 + (int)(Math.random() *10);
		
		System.out.println("Welcome to the Guessing game\nEnter a digit from 0 to 10:");
		Usernumber = input.nextInt();
		if (computerNumber == Usernumber)
		{
			System.out.println("You Guessed the right number");
			System.out.printf("Your number %d, Random number %d" , Usernumber, computerNumber);
		}

		else
			{
				if (computerNumber < Usernumber)
				{
					System.out.println("You Guessed to High");
					System.out.printf("Your number %d, Random number %d" , Usernumber, computerNumber);
				}
				else
				{	System.out.println("You Guessed to Low");
				System.out.printf("Your number %d, Random number %d" , Usernumber, computerNumber);
				}	
			}

}
	//End main

}
	//End class
