# Add-two-complex-numbers-in-java
Add two complex numbers in java
public class ComplexNumber{
    //for real and imaginary parts of complex numbers
    double real, img;
 
    //constructor to initialize complex numbers
    ComplexNumber(double r, double i){
        this.real = r;
        this.img = i;
    }
 
    public static ComplexNumber sum(ComplexNumber c1, ComplexNumber c2)
    {
        //create a temporary complex number to hold the sum of two numbers
        ComplexNumber temp = new ComplexNumber(0, 0);
 
        temp.real = c1.real + c2.real; //plus real parts
        temp.img = c1.img + c2.img; //plus imaginary parts
 
        //return the output complex number
        return temp;
    }
    public static void main(String args[]) {
        ComplexNumber c1 = new ComplexNumber(5.2, 4.4); //enter the real and imaginary parts of the first complex number
        ComplexNumber c2 = new ComplexNumber(2.0, 7.3); //enter the real and imaginary parts of the second complex number
        ComplexNumber temp = sum(c1, c2);
        System.out.printf("Result is: "+ temp.real+" + "+ temp.img +"i"); //display result on screen
    }
}
