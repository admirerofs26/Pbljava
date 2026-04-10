1.	Create a class Laptop with private fields brand and price. Write a constructor that initializes both fields.  Write getter methods for both. Write a method displaySpecs() that prints the brand and price. In main, create one Laptop object and call displaySpecs().

class Laptop {
    private String brand;
    private double price;

    Laptop(String brand, double price) {
        this.brand = brand;
        this.price = price;
    }
    
    String getBrand() {
        return brand;
    }

    double getPrice() {
        return price;
    }

    void displaySpecs() {
        System.out.println("Brand: " + brand);
        System.out.println("Price: " + price);
    }
}

public class Main {
    public static void main(String[] args) {
        Laptop l = new Laptop("Dell", 75000);
        l.displaySpecs();
    }
}












2.Design a class Mobile having two private attributes: modelName and batteryLife. Use a constructor with parameters and the this keyword to assign values. Provide methods to get each attribute and a method to print all details. Test the class by creating an object in main.

class Mobile {
    private String modelName;
    private int batteryLife;

    Mobile(String modelName, int batteryLife) {
        this.modelName = modelName;
        this.batteryLife = batteryLife;
    }

    String getModelName() {
        return modelName;
    }

    int getBatteryLife() {
        return batteryLife;
    }

    void printDetails() {
        System.out.println("Model: " + modelName);
        System.out.println("Battery Life: " + batteryLife + " hours");
    }
}

public class Main {
    public static void main(String[] args) {
        Mobile m = new Mobile("Samsung Galaxy", 24);
        m.printDetails();
    }
}













3.Write a class Television with private variables screenSize and type. The constructor should take values for both and use this. Add getters and a method showDetails(). In main, create one Television object and show its details.

class Television {
    private int screenSize;
    private String type;

    Television(int screenSize, String type) {
        this.screenSize = screenSize;
        this.type = type;
    }

    int getScreenSize() {
        return screenSize;
    }

    String getType() {
        return type;
    }

    void showDetails() {
        System.out.println("Screen Size: " + screenSize + " inches");
        System.out.println("Type: " + type);
    }
}

public class Main {
    public static void main(String[] args) {
        Television t = new Television(55, "LED");
        t.showDetails();
    }
}













4.Build a class Fan that contains private data members speed and color. The constructor must assign values using this. Write a method describe() that prints both values. In main, instantiate the class and call describe().

class Fan {
    private int speed;
    private String color;

    Fan(int speed, String color) {
        this.speed = speed;
        this.color = color;
    }

    void describe() {
        System.out.println("Speed: " + speed);
        System.out.println("Color: " + color);
    }
}

public class Main {
    public static void main(String[] args) {
        Fan f = new Fan(3, "White");
        f.describe();
    }
}



















5.Create a class Bottle with private fields capacity and material. Write a constructor that uses this to resolve naming conflicts. Add getters and a method info(). In main, create one Bottle object and print its information.

class Bottle {
    private int capacity;
    private String material;

    Bottle(int capacity, String material) {
        this.capacity = capacity;
        this.material = material;
    }

    int getCapacity() {
        return capacity;
    }

    String getMaterial() {
        return material;
    }

    void info() {
        System.out.println("Capacity: " + capacity + " ml");
        System.out.println("Material: " + material);
    }
}

public class Main {
    public static void main(String[] args) {
        Bottle b = new Bottle(1000, "Steel");
        b.info();
    }
}

6.Write a Java program using a for loop to print all odd numbers from 1 to 10.

public class Main {
    public static void main(String[] args) {
        for (int i = 1; i <= 10; i += 2) {
            System.out.println(i);
        }
    }
}



7.Write a program that uses a do-while loop to print numbers from 10 down to 1.

public class Main {
    public static void main(String[] args) {
        int i = 10;
        do {
            System.out.println(i);
            i--;
        } while (i >= 1);
    }
}

8.Write a Java program that takes a number from the user and prints its multiplication table from 1 to 10 using a for loop.

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();

        for (int i = 1; i <= 10; i++) {
            System.out.println(n + " x " + i + " = " + (n * i));
        }
    }
}

9.Write a program that keeps asking the user to enter a positive number until they do. Use a while loop for this.

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = 0;

        while (n <= 0) {
            n = sc.nextInt();
        }

        System.out.println("Positive number entered: " + n);
    }
}



10.Write a Java program to find the factorial of a number entered by the user using a for loop. Factorial of 5 is 5×4×3×2×1 = 120.

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int fact = 1;

        for (int i = 1; i <= n; i++) {
            fact *= i;
        }

        System.out.println("Factorial: " + fact);
    }
}


11.Write a Java program that converts a float value 55.75 into an int and prints both. Also show automatic conversion from char to int.

public class Main {
    public static void main(String[] args) {
        float f = 55.75f;
        int i = (int) f;

        char ch = 'A';
        int ascii = ch;

        System.out.println("Float value: " + f);
        System.out.println("Converted int: " + i);
        System.out.println("Char value: " + ch);
        System.out.println("Char to int: " + ascii);
    }
}

12.Take a long value 1000 and convert it into an int explicitly. Print both values. Also show how a byte value automatically fits into a short variable.

public class Main {
    public static void main(String[] args) {
        long l = 1000;
        int i = (int) l;

        byte b = 50;
        short s = b;

        System.out.println("Long value: " + l);
        System.out.println("Converted int: " + i);
        System.out.println("Byte value: " + b);
        System.out.println("Byte to short: " + s);
    }
}

13.Write a program that demonstrates converting a double 45.67 to an int (data loss happens). Also show how an int automatically becomes a long.

public class Main {
    public static void main(String[] args) {
        double d = 45.67;
        int i = (int) d;

        int x = 100;
        long l = x;

        System.out.println("Double value: " + d);
        System.out.println("Converted int: " + i);
        System.out.println("Int value: " + x);
        System.out.println("Int to long: " + l);
    }
}

14.Convert the value 3.14159 from double to float using explicit casting. Print both. Also show automatic conversion from int to double.

public class Main {
    public static void main(String[] args) {
        double d = 3.14159;
        float f = (float) d;

        int x = 10;
        double d2 = x;

        System.out.println("Double value: " + d);
        System.out.println("Converted float: " + f);
        System.out.println("Int value: " + x);
        System.out.println("Int to double: " + d2);
    }
}




15.Write a program that shows what happens when you convert a large int (like 300) into a byte. Print the original and the converted value.

public class Main {
    public static void main(String[] args) {
        int x = 300;
        byte b = (byte) x;

        System.out.println("Original int: " + x);
        System.out.println("Converted byte: " + b);
    }
}

16.Write a Java program that takes two numbers from the user and divides them. Use try-catch to handle the situation when the user enters zero as the second number. Print "Invalid denominator" in the catch block.

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        int b = sc.nextInt();

        try {
            int result = a / b;
            System.out.println("Result: " + result);
        } catch (ArithmeticException e) {
            System.out.println("Invalid denominator");
        }
    }
}


17.Create a program that asks the user to enter an array index. Access an element from an array of size 5. Use try-catch to handle ArrayIndexOutOfBoundsException and print "Index out of range".

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        int[] arr = {10, 20, 30, 40, 50};
        Scanner sc = new Scanner(System.in);

        int index = sc.nextInt();

        try {
            System.out.println("Element: " + arr[index]);
        } catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("Index out of range");
        }
    }
}

18.Write a program that converts a string to an integer using Integer.parseInt(). Use try-catch to handle NumberFormatException if the user enters something that is not a number. Print "Invalid number format".

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String input = sc.nextLine();

        try {
            int num = Integer.parseInt(input);
            System.out.println("Number: " + num);
        } catch (NumberFormatException e) {
            System.out.println("Invalid number format");
        }
    }
}

19.Take two numbers from the user. If the second number is zero, throw an ArithmeticException manually using the throw keyword and catch it to print "Cannot divide by zero".

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        int b = sc.nextInt();

        try {
            if (b == 0) {
                throw new ArithmeticException();
            }
            int result = a / b;
            System.out.println("Result: " + result);
        } catch (ArithmeticException e) {
            System.out.println("Cannot divide by zero");
        }
    }
}


20.Write a program that reads a number from the user. If the number is negative, create and throw a custom exception called NegativeNumberException (just declare this exception class). Catch it and print "Negative numbers not allowed".

import java.util.Scanner;

class NegativeNumberException extends Exception {
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();

        try {
            if (n < 0) {
                throw new NegativeNumberException();
            }
            System.out.println("Number: " + n);
        } catch (NegativeNumberException e) {
            System.out.println("Negative numbers not allowed");
        }
    }
}
