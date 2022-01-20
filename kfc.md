---
layout: page
title: KFC SubGroup Tech Terms
subtitle: Kira Liao, Flora Yuan, Calvin Cheah (KFC)
---
## 1. Casting, specifically for Division
_Definition:_ Casting - Assigning a variable to a specific data type

_Example:_
```javascript
double d = num / (double) denom;
```

## 2. Casting, specifically for Truncating or Rounding
_Definition:_ Assigning a variable to a specific data type

_Example:_
```javascript
(int)(99.9999) → Value of 99
```

## 3. Wrapper Classes, why wrap int, double
_Definition:_ Wrapper classes provide a way to use primitive data types (int, boolean, etc..) as objects.

_Example:_
```javascript
ArrayList<int> myNumbers = new ArrayList<int>(); // Invalid
ArrayList<Integer> myNumbers = new ArrayList<Integer>(); // Valid
```

## 4. Concatenation, rules on mixed type Concatenation


## 5. Math class, specifically Random usage
_Definition:_ The class Math contains methods for performing basic numeric operations such as the elementary exponential, logarithm, square root, and trigonometric functions.

_Example:_
```javascript
double a = Math.random(); //generates number from 0 to 1 (but not 1)
```

## 6. Compound Boolean Expression
_Definition:_ 
- == equals
- != does not equal
- < less than
- greater than is ">"
- greater than or equal to is ">="
- <= less than or equal to

## 7. Truth Tables
_Definition:_ How two logical conditions are combined based on AND, OR, and NOT
![truthtable](/assets/img/truthtable.png)

## 8. De Morgan's Law
_Definition:_ 
- Not (A and B) is the same as Not A or Not B.
- Not (A or B) is the same as Not A and Not B.
- The || is "or" and && is and. For ||, either statement has to be true in order for the boolean to be true, and for && both statements have to be true in order for the boolean to be true.

## 9. Comparing Numbers
_Definition:_ Primitive variables compared using ==, also known as the equality operator, should be compatible between argument types

[_Example:_](https://github.com/florayuan18/pikachudrinkingwindex/blob/2ddbc249a430fbb2aad434a02a9b88e93763c8c4/src/main/java/com/example/sping_portfolio/controllers/CalvinAboutMVC/CalvinFRQ/FRQ_3/FRQ3_P1.java#L34-L39)

## 10. Comparing Strings
## 11. Comparing Objects
_Definition:_ Using the equals() method

## 12. for loop, enhanced for loop
_Definition:_
- Repeats a specific block of code for known number of times
- Parts: initialization, Boolean expression, and increment
- If true, loop executes statements in body | If false, exit for loop

_Example:_
``` javascript
public static void main(String[] args)
{
	
for (int num = 1; num <= 10; num++)
	{
		System.out.println(num+1);
	}
	System.out.println(“Loop Completed”);
}
```

## 13. while loop versus do while loop
_Definition:_
- Executed based on a given Boolean condition
- If true, loop continues | If false, loop stops
- Condition can be specified | while (number > 100)

_Example:_
``` javascript
public static void main(String[] args)
{
    int value = 1;
    while (value <= 10)
    {
        System.out.println(value+1);
        value++;
    }
    System.out.println(“Loop Completed”);
}
```

## 14. nested loops
_Definition:_ One loop inside another loop

[_Example:_](https://github.com/florayuan18/pikachudrinkingwindex/blob/2ddbc249a430fbb2aad434a0[…]tfolio/controllers/CalvinAboutMVC/CalvinFRQ/FRQ_4/CoinGame.java)

## 15. Big O notation (Hash map, Binary Search, Single loop, Nested Loop)
_Definition:_ 
- n^2 -> nested for loop
- Can calculate how long it takes a loop to find "i"
- Time complexity, used instead of raw time, used to help find the most efficient algorithm
- How long it would take relative to the data input/size

## 16. Creating a Class, describe Naming Conventions
_Definition:_
- Naming conventions: capital letters instead of a space
- Methods: lowercase and capital (camel case)

## 17. Constructor, describe why there is no return
_Definition:_ Constructor is a non-static method with name <init> and void return type. It does not return anything.

## 18. Accessor methods, relationship to getter
_Definition:_ “Getters” retrieve information about an object

## 19. Mutator methods, relationship to setter, describe void return type
_Definition:_ “Setters” replace information about an object

## 20. Static variables, Class variables
_Definition:_ Declared with the static keyword

## 21. Static methods, Class methods
_Definition:_ Methods that can be called without creating on object of class. For example, the main() method. They can only call other static methods.

## 22. this Keyword
_Definition:_
- Using standard convention of the instance variable
- dist.name=name
- Need to use “this”

## 23. main method, tester methods
_Definition:_ Tester methods - Used in console running, public static void main(String[] args)

## 24. Inheritance, extends
_Definition:_
- One class (sub class) inherits the features of another class (super class)
- Reusing existing information in classes for other classes
- Uses the word **extends**

_Example:_
``` javascript
public class Animal{
// information goes here
}
public class Dog extends Animal{
}
```

## 25. Subclass constructor, super Keyword
_Definition:_ If the method overrides the superclass’s methods, overridden method can be invoked using the keyword _super_

_Example:_
``` javascript
public void printMethod() {
     super.printMethod();
     System.out.println("Printed in Subclass");
}
```

## 26. Overloading a method, same name different parameters
_Definition:_
- Two of more methods of the same name in class, also known as compiletime polymorphism
- Can be used to invoke different parameters

_Example:_
``` javascript
class Dog{
    public void bark(){
        System.out.println("woof ");
    }
 
    //overloading method
    public void bark(int num){
    	for(int i=0; i<num; i++)
    		System.out.println("woof ");
    }
}
```

## 27. Overriding a method, same signature of a method
_Definition:_
- When a method in a subclass has the same name, same parameters or signature, and same return type - method in subclass overrides the superclass
- Overriding lets child class implement a method already in the parent class
- Also known as runtime polymorphism
- Known as method hiding if static method is defined with same signature in base class

_Example:_
``` javascript
public class Drink{
    public static void testClassMethod() {
        System.out.println("The static method in Drink");
    }
    public void testInstanceMethod() {
        System.out.println("The instance method in Drink");
    }
}


public class Boba extends Drink{
    public static void testClassMethod() {
        System.out.println("The static method in Boba");
    }
    public void testInstanceMethod() {
        System.out.println("The instance method in Boba");
    }
```

## 28. Abstract Class, Abstract Method
_Definition:_
- **Abstract Class**: hide implementation complexities by providing functionalities on a simpler interface
- **Abstract Method**: 
  - A method with no body (implementation)
  - Rules: 1) no body, 2) classes that have abstract methods should be declared abstract, 3) extending abstract class - must implement abstract parent class

_Example:_
``` javascript
public abstract int pikachu(int n1, int n2);
```

## 29. Object superclass methods: toString(), compare(), clone()
_Definition:_
- **toString()**: representing an object as a string - readable to human
  - When printing an object, Java invokes toString() method - returns String representation of object
  - Overriding toString() method - able to return value of object

_Example:_
Without toString():
``` javascript
public static void main(String args[]){  
   Student s1=new Student(101,"Calvin","pikachu");  
   Student s2=new Student(102,"Kira","windex");  
     
   System.out.println(s1);//compiler writes here s1.toString()  
   System.out.println(s2);//compiler writes here s2.toString()  
```
Prints out Hash

With toString():
``` javascript
public String toString(){//overriding the toString() method  
return rollno+" "+name+" "+city;  
}  
public static void main(String args[]){  
   Student s1=new Student(101,"Calvin","pikachu");  
   Student s2=new Student(102,"Kira","windex");  

System.out.println(s1);//compiler writes here s1.toString()  
System.out.println(s2);//compiler writes here s2.toString()  
}
```
Prints:
101 Calvin pikachu
102 Kira windex

- **compare()**: compares two class-specific objects
  - 0: if (x==y)
  - -1: if (x < y)
  - 1: if (x > y)

_Example:_
``` javascript
System.out.println(Integer.compare(x, y));
int w = 15;
int z = 8;
```
Prints 1 because 15 > 8

- **clone()**: creating an exact copy of an object - new instance but same contents initialized
  - Changes on one (shallow copy) will be reflected on another
  - Deep copy - copies fields and makes copies - dynamically allocated memory
  - Advantages: if copy constructor is used - data has to be copied explicitly
    - Many have to reassign all fields
      Cloning avoids the extra processing

_Example:_
``` javascript
 Test c = new Test();
 
    public Object clone() throws CloneNotSupportedException
    {
        // Assign the shallow copy to
        // new reference variable t
        Test2 t = (Test2)super.clone();
 
        // Creating a deep copy for c
        t.c = new Test();
        t.c.x = c.x;
        t.c.y = c.y;
```

## 30. Late binding of object, referencing superclass object, ie Animal a = new Chicken(); Animal b = new Goat();
_Definition:_
- Type is unknown until variable is exercised during runtime (decided at runtime)
- How polymorphism is implemented, dynamic types
- Example: Overriding  both parent and child classes have same method

_Example:_
``` javascript
public class NewClass {
    public static class superclass {
        void print()
        {
            System.out.println("print in superclass.");
        }
    }
  
    public static class subclass extends superclass {
        @Override
        void print()
        {
            System.out.println("print in subclass.");
        }
    }
```

## 31. Polymorphism: any of overloading, overriding, late binding
_Definition:_
- Ability of an object to take many forms
- Same action in multiple ways
- Compile-time polymorphism (method overloading) and run time polymorphism

_Runtime Polymorphism Example:_
Animal.java
``` javascript
public class Animal{
   public void sound(){
      System.out.println("Animal is making a sound");   
   }
}
```

Horse.java
``` javascript
class Horse extends Animal{
    @Override
    public void sound(){
        System.out.println("Neigh");
    }
    public static void main(String args[]){
    	Animal obj = new Horse();
    	obj.sound();
    }
}
```

_Compile Time Polymorphism Example:_
``` javascript
class Overload
{
    <filler code yeah>
}
class MethodOverloading
{
    public static void main (String args [])
    {
        Overload Obj = new Overload();
        double result;
        Obj .demo(10);
        Obj .demo(10, 20);
        result = Obj .demo(5.5);
        System.out.println("O/P : " + result);
    }
}
```


## 32. Web API, REST, FETCH, Async, Request, Response
## 33. CRUD