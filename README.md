# 34-.Interface-calculator-
package pkginterface.calculator;
import java.util.Scanner;
interface Calculator{
    double add(double a, double b);
    double subtract(double a,double b);
    double multiply(double a,double b);
    double divide(double a,double b);
}
class SimpleCalculator implements Calculator{

    @Override
    public double add(double a, double b) {
        return a+b;
    }

    @Override
    public double subtract(double a, double b) {
        return a-b;
    }

    @Override
    public double multiply(double a, double b) {
        return a*b;
    }

    @Override
    public double divide(double a, double b) {
    return a/b;
    }
   
}

/**
 *
 * @author 1BSCCSA22
 */
public class INTERFACECALCULATOR {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Scanner scanner = new Scanner(System.in);
        Calculator calculator = new SimpleCalculator();
        System.out.println("welcome to the simple calculator!");
        System.out.println("enter the first number:");
        double num1 = scanner.nextDouble();
        System.out.println("enter the second number:");
        double num2 = scanner.nextDouble();
        System.out.println("\nresult:");
        System.out.println("addition:" +calculator.add(num1, num2));
        System.out.println("subtraction:" +calculator.subtract(num1,num2));
        System.out.println("multiplication:" +calculator.multiply(num1, num2));
        System.out.println("division:" +calculator.divide(num1, num2));
        scanner.close();
    }
    
}

Output:
welcome to the simple calculator!
enter the first number:
23
enter the second number:
12
Result:
addition:35.0
subtraction:11.0
multiplication:276.0
division:1.9166666666666667
BUILD SUCCESSFUL (total time: 12 seconds)


