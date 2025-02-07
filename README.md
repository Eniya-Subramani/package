# package
package math_operations;
 class Calculator{
    public int add(int a,int b){
        return a+b;
    }
    public int subtract(int a,int b){
        return a-b;
    }
    public int multiply (int a,int b){
        return a*b;
    }
    public double divide(int a,int b){
        if(b!=0){
            return(double)a/b;
        }else{
            System.out.println("cannot divide by zero!");
            return Double.NaN;
        }
                
    }
    
}
//mathutils class in the math_operations package
 class MathUtils{
     public double CalculateSquareRoot(double num){
         if(num>=0){
             return Math.sqrt(num);
         }else{
             System.out.println("cannot calculate square root of a negative number !");
             return Double.NaN;
         }
     }
 }
public class Math_operations {
    public static void main(String[] args) {
        // TODO code application logic here
        // Create instances from the math_operations package
math_operations.Calculator calculator = new math_operations.Calculator();
math_operations.MathUtils mathUtils = new math_operations.MathUtils();
// Perform basic mathematical operations
System.out.println("Addition: " + calculator.add(5, 3));
System.out.println("Subtraction: " + calculator.subtract(8, 4));
System.out.println("Multiplication: "+ calculator.multiply(2, 6));
System.out.println("Division: "+ calculator.divide(10, 2));
// Calculate square root
System.out.println("Square Root: " +mathUtils.CalculateSquareRoot(25));
System.out.println("Square Root of -9:" + mathUtils.CalculateSquareRoot(-9));
    }
    
}

Output:

Addition: 8
Subtraction: 4
Multiplication: 12
Division: 5.0
Square Root: 5.0
cannot calculate square root of a negative number !
Square Root of -9:NaN

