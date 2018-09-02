# reverse-number1
enter number and then reverse number without string method
import java.util.Scanner;
public class ReverseNumber{

     public static void main(String []args){
        Scanner sc = new Scanner(System.in);
        
        System.out.println("Enter the Number to be Reversed: ");
        int num = sc.nextInt();
        
        System.out.println("Reversed Number is: " + reversedNumber(num) );
     }
    
    
     
	public static int reversedNumber(int num) {
		
		//Assuming there is no intial zeroes present
		
		
		int sum = 0;
        int digit = 0;
		while (num > 0) {

			digit = num % 10;
			sum = (sum * 10) + digit;
			num = num / 10;
		}
		
		
		return sum ;
		
		

	}
}

