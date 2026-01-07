# Java Lab Programs

## Experiment 1 – Default Value
public class DefaultValues {
    byte b;
    short s;
    int i;
    long l;
    float f;
    double d;
    char c;
    boolean bool;

    public static void main(String[] args) {

        DefaultValues obj = new DefaultValues();

        System.out.println("the Default value of byte is  : " + obj.b);
        System.out.println("the Default value of short is : " + obj.s);
        System.out.println("the Default value of int  is  : " + obj.i);
        System.out.println("the Default value of long is  : " + obj.l);
        System.out.println("the Default value of float is : " + obj.f);
        System.out.println("the Default value of double is: " + obj.d);
        System.out.println("the Default value of char  is : '" + obj.c + "'");
        System.out.println("the Default value of boolean is : " + obj.bool);
    }
}
### Output
![Program Output](1(a)output.png)
