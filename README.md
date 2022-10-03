# PP-2.11


/* 

10/2/2022

 Derek Durand

Converts dollars to bills and change

*/ 
import java.util.Scanner;

public class PP211 {

   
    public static void main(String[] args) {
        int tens, fives, ones, quarters, dimes, nickles, pennies, amount;    
        
        Scanner sc = new Scanner(System.in);
        
        System.out.print("Input Dollar amount: ");
        float dollarAmount = sc.nextFloat();
        
         amount = (int) (dollarAmount * 100);
         
        tens=amount/1000;
        amount%=1000;                         
        fives = amount / 500;    
        ones=amount/100;                  
        amount%=100;
        quarters=amount/25;
        amount%=25;
        dimes=amount/10;
        amount%=10;
        nickles=amount/5;
        pennies=amount%5;
        
        System.out.println(tens +" ten dollar bills");

        System.out.println(fives +" five dollar bills");

        System.out.println(ones +" one dollar bills");

        System.out.println(quarters +" quarters");

        System.out.println(dimes +" dimes");

        System.out.println(nickles +" nickles");

        System.out.println(pennies +" pennies");
        
    
    
    
    
    }
}
