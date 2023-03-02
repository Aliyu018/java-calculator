package javaapplication1;
import java.util.Scanner;
public class JavaApplication1 {

  
    public static void main(String[] args) {
        int choice;
        double a,b,result;
        do
        {
        Scanner Read=new Scanner(System.in);
        System.out.println("******************&&&&&&");
        System.out.print("1.Addition\n2.multiplication\n3.power\n4.square Root\n5.exit\nchoose(1-5");
        choice=Read.nextInt();
        choice=Integer.parseInt(JOptionPane.showInputDialog("1.+\n2. *\n3. ^\n4. \n5.Exit make your choice"));
        switch(choice)
        
        {
            case 1:System.out.print("enter the first number:");
                   a=Read.nextDouble();
                   System.out.print("Enter second number:");
                   b=Read.nextDouble();
                   result= a+b;
                   System.out.println(a+"*"+b+"="+result);
                    break;
            case 2:System.out.print("enter the first number:");
                   a=Read.nextDouble();
                   System.out.print("Enter second number:");
                   b=Read.nextDouble();
                   result= a-b;
                   System.out.println(a+"*"+b+"="+result);break;
            case 3:System.out.print("enter the first number:");
                   a=Read.nextDouble();
                   System.out.print("Enter second number:");
                    b=Read.nextDouble();
                   result=Math.pow(a, b);
                   System.out.println(a+"*"+b+"="+result);break;
            case 4:System.out.print("enter the first number:");
                   a=Read.nextDouble();
                   System.out.print("Enter second number:");
                   result=Math.sqrt(a);
                   System.out.println("square Root of"+a+"="+result);
                   break;
            case 5:break;
                  
            default:System.out.println("you made a mistake");
            
        }
        
    }  while(choice !=5);
    
}
}
