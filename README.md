# prime-number-using-methods
import java.util.Scanner;
public class Main
{
	public static void main(String[] args) {
	    
		System.out.print("Enter the interval 1:");
		Scanner a = new Scanner(System.in);
		int x = a.nextInt();
		System.out.print("Enter the interval 2:");
	   int y =a.nextInt();
	   printBetween(x,y);
	}
		
		
    public static boolean isPrime(int input){
        int count =0;
		for(int i=1;i<=input;i++){
		    if (input%i==0)
		    count = count + 1;
		    
		}
		if (count==2)
		    //System.out.print("prime");
		    return true;
	
	  return false;
	  
	}
	public static void printBetween(int start,int end){
	    for(int i=start;i<=end;i++){
	       if (isPrime(i))
	       System.out.print(i+" ");
	    }
	}
}
