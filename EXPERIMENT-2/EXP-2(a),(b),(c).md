#EXPERIMENT 2
##EXPERIMENT-2A TITLE:implement class mechanism in java
```
class Square {

    void area(int length) {
        System.out.println("The area of square: " + (length * length));
    }

    void perimeter(int length) {
        System.out.println("The perimeter of square: " + (4 * length));
    }
}
public class squ {

    public static void main(String[] args) {

        Square obj = new Square();

        obj.area(5);
        obj.perimeter(6);
    }
}

```

#OUTPUT:
![EXPERIMENT 2A OUTPUT](2(a)output.png)





#EXPERIMENT2B
##EXP2B TITLE:implement method overloading
```
class Overload {

    void add(int a, int b) {
        System.out.println("Result of adding two integers: " + (a + b));
    }

    void add(double a, double b) {
        System.out.println("Result of adding two double values: " + (a + b));
    }

    void add(int a, int b, int c) {
        System.out.println("Result of adding three integers: " + (a + b + c));
    }
}
public class overloading {

    public static void main(String[] args) {

        Overload obj = new Overload();

        obj.add(5, 10);
        obj.add(2.5, 6.5);
        obj.add(5, 10, 15);
    }
}
```
#OUTPUT:
![EXP2B OUTPUT](2(b)output.png)



