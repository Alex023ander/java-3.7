# java-3.7
//Reads the lengths of the sides of a triangle from the user and computes the area using Heron's formula.

import java.text.DecimalFormat;
import java.util.Scanner;
public class Comp37 {


    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        DecimalFormat fmt = new DecimalFormat("0.###");
      double a, b, c, s;
      double area;
      
      
      System.out.println("Enter side a: ");
      a = scan.nextDouble();
      
      System.out.println("Enter side b: ");
      b = scan.nextDouble();
      
      System.out.println("Enter side c: ");
      c = scan.nextDouble();
      
      s = ((a + b + c)/2);
      
      area = (Math.sqrt(s * (s-a) * (s-b) * (s-c)));
      
      System.out.println("Area = " + fmt.format(area));
              
    }
    
}
