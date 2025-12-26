# JAVALAB

# Expt-1a
```java
class Test {
    byte b;
    int i;
    float f;
    char c;
    double d;
    long l;
    short s;
    boolean bl;

    public static void main(String[] args) {
        Test t = new Test();
        System.out.println(t.b);
        System.out.println(t.i);
        System.out.println(t.f);
        System.out.println(t.c);
        System.out.println(t.d);
        System.out.println(t.l);
        System.out.println(t.s);
        System.out.println(t.bl);
        
    }
}

```
#output:
![output of primitive](primitive.jpeg)

# Expt-1b
```java
import java.util.Scanner;

class QuadraticRoots {
    public static void main(String[] args) {

        double a, b, c, D;
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter value of a: ");
        a = sc.nextDouble();

        System.out.print("Enter value of b: ");
        b = sc.nextDouble();

        System.out.print("Enter value of c: ");
        c = sc.nextDouble();

        D = b * b - 4 * a * c;
        System.out.println("Discriminant (D) = " + D);

        if (D > 0) {
            double x1 = (-b + Math.sqrt(D)) / (2 * a);
            double x2 = (-b - Math.sqrt(D)) / (2 * a);

            System.out.println("Roots are real and distinct.");
            System.out.println("Root 1 = " + x1);
            System.out.println("Root 2 = " + x2);

        } else if (D == 0) {
            double x = -b / (2 * a);
            System.out.println("Roots are real and equal.");
            System.out.println("Root = " + x);

        } else {
            double real = -b / (2 * a);
            double imaginary = Math.sqrt(-D) / (2 * a);

            System.out.println("Roots are imaginary (complex).");
            System.out.println("Root 1 = " + real + " + i" + imaginary);
            System.out.println("Root 2 = " + real + " - i" + imaginary);
        }

        sc.close();
    }
}
```
#output:
![output of Quadratic](quadratic.jpeg)
