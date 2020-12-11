<!--
Author: peena5370 
Created: 18 October 2020
-->

### Java Comments(Java 注释)
```java
/* many lines  
 * line 1
 * line 2
 * line 3
 * line 4
 * comments */
// this is single line comment
```

### Java Annotation
```java
@Override
//use for tell compiler to check error for rewrite code syntax
@Deprecated
//use for check class, method, interface wether it is expired and throw error 
@SuppressWarnings({"keywords"})
//suppress warning that trigger with keywords(all,boxing,cast,dep-ann,deprecation,fallthrough,finally,hiding....)
@SafeVarargs
@FunctionalInterface
```

### Variable Declaration
```java
String textString = "string here";
int iValue = 1000, iValue2 = 200, iValue3 = 4000;
float fValue = 1000.00, fValue2, fValue3 = 19.99;
char cChar = 'A', cChar2 = 'B';
boolean x = true, y = false;	//boolean = true / false
Others datatype = byte, short, int, long, float, double, boolean, char
String, Arrays(new Arrays), Classes(declare class),Interface(interface class)
```

### Input 
```java
import java.util.Scanner;
//declare datatype
int iValue = new Scanner(System.in).nextInt();
variableName = new Scanner(System.in).read value type();
nextInt() = // read int value, nextFloat() = read float value, 
nextDouble() = // read double value
next() = //read string before whitespace, nextLine() = read entire string
nextBoolean = // read true or false value
```

### Output
```java
System.out.println(textString + iValue + fValue + x + y);
System.out.printf("%2.2f\n",x);		
//new type for output value or strings(same with C)
```

### Operators(calculation)
```java
/* Calculation symbol */
Val = x + y;
Val = x - y:
Val = x * y;
Val = x / y;
Val = x % y;
x++ / ++x / x-- /--x;
x = 5;
x += 5 / x = x + 5;
x -= 5 / x = x - 5;
x *= 5 / x = x * 5;
x /= 5 / x = x / 5;
x %= 5 / x = x % 5;
x &= 5 / x = x & 5;
x |= 5 / x = x | 5;
x ^= 5 / x = x ^ 5;
x >>= 5 / x = x >> 5;
x <<= 5 / x = x << 5;

/* Comparison symbol */
x == y;		// equal to 
x != y;		// not equal to
x > y;		// bigger than
x < y;		// smaller than 
x >= y;		// bigger or equal to 
x <= y;		// smaller or equal to

/* Logical symbol */
x = 5 && x = 10		// logical and
x = 5 || x <9		// logical or
!(x <5 && x <10)	// logical not(return false if result true)

/* Bitwise symbol(for binary calculation use) */
&		// AND
|		// OR
~		// NOT
^		// XOR
<<		// zero-fill left shift
>>		// signed right shift
>>>		// zero-fill right shift
```

### String Conversion
```java
String newStr = "Test string for output";
System.out.println(newStr.toUpperCase());	// string to upper case
System.out.println(newStr.toLowerCase());	// string to lower case
System.out.println(newStr.indexOf("string"));	
//return string location value(first string output first) output = 5

/* Input Symbol */
\'		// single quote
\"		// double quote
\\		// backslash

/* Escape Tag */
\n		// newline
\r		// carriage return
\t		// tab
\b		// backspace
\f		// form feed
```

### Math Class
```java
Math.max(val1, val2);		// find highest value between val1 and val2
Math.mix(val1, val2);		// find smallest value between val1 and val2
Math.sqrt(val);				// square root of val
Math.abs(-4.7);				// return positive value of value
Math.random();				
// return random number between a range 0 to max number
```

### Condition Statements
```java
/* if...else */
if( x == 1) {
	// code statements
}
else {
	// code statements
}

/* if...else if...else */
if ( x == 1) {
	// code statements
}
else if ( x == 2) {
	// code statements 
}
else {
	// code statements
}

/* short form if...else */
variable = ( x == 1) ? expressionTrue : expressionFalse;	
//variable = String output, expressionTrue = functionName1()/"output 1", expressionFalse = functionName2()/"output2";

/* switch...case */
int iValue = 4;
switch(iValue) {
	case 1:
		// code statements;
		break;
	case 2:
		// code statements;
		break;
	case 3:
		// code statements;
		break;
	case 4:
		// code statements;
		break;
	case 5:
		// code statements;
		break;
	default:
		// code statements;
}

/* while loop */
while ( x < 6 ) {
	// code statements;
	value ++;
}

/* do...while */
do {
	// code statements
}while ( x < 6 );

/* for loop */
for( x = 0; x < 5; x++) {
	// code statements
}

/* nested for loop */
for( x = 0; x < 5; x++) {
    // code statements
	for( y = 0; y < 5; y++) {
		// code statements
	}
}

/* For-Each loop (use to loop elements through array) */
String[] text = {"Str1","Str2","Str3"};
for(String newVar : text) {		
// for( datatype variableName : arrayName) {}
	// code statements(output newVar);
}

/* break / continue */
for(x=0; x<10; x++){
	if(x==4){
    // break entire loop if condition = true
	break;
	}
}
for(x=0; x<10; x++){
	if(x==4){
        // break only one loop based on the condition 
		continue;
	}
}
```

### Arrays
```java
// array declaration(datatype[] arrayName)
String[] cars;
// 1D array
String[] cars = {"Str1","Str2","Str3"};
// 2D array
int[][] newArr = { {1,2,3,4},{5,6,7,8}};
// output length of cars array
cars.length

/* for loop array */
for( int i = 0; i < newArr.length; i++) {
	for( int j = 0; j < newArr[i].length; j++) {
		// code statements
	}
}
```

### Call Function Method
```java
/* declaring new function */
// declare new function in same class
static void newFunc() {
	// code statements;
}

public static void main(String[] args) {
	// execute function in main() function	
    newFunc();
}

/* declare function with parameters */
static void funcText( String newTxt) {
	System.out.println(newTxt + " newStr");
}

public static void main(String[] args) {
	// declare value for function(output = Str1 newStr)
	funcText("Str1");		
	// output = Str2 newStr
	funcText("Str2");
}

/* return function value */
static void newFunc( int x, y) {
	return x + y;
	
	public static void main(String[] args) {
		int z = newFunc(5,3);
        // output 8(5 + 3)
		System.out.println(z);
	}
	
/* if else return statement */
static void diffFunc(int x) {
	if (x == 5) {
		// code statement 1;
	}
	else {
		// code statement 2;
	}
}

public static void main(String[] args) {
    // execute code statement 2
	diffFunc(10);
}
```

# Java OOP
* make new class file is similar like declare universal variable, then reuse in other .java file,
* declare public class to make it usable at other places,
* then use pointer to access the items we need such as (newObj.x --> object.other class variables) 
* before use at other .java file, need to declare as new class( otherClass newObj = new otherClass();  newObj.otherClassFunc();

```java
/* Create class */
// declaring a class with name NewClass
public class NewClass {
	int i = 5;
	public static void main(String[] args){
        //declaring object call newObj
        NewClass newObj = new NewClass();
        // output value of i
        System.out.println(newObj.i);
}

/* create class with other .java folder */
subClass.java
public class subClass {
	// final use to declare fixed value to prevent override
	final int i = 10;
	int j = 5;
}

mainClass.java 
class mainClass {
	public static void main(String[] args) {
		subClass newObj = new subClass();
        // output 5
		System.out.println(newObj.j);
	}
}

/* class and object modifier */
//public = can be access by all classes
// private = only can access in own class
// default/empty declaration = only accessible in same package
// protected = accessible in same package and subclasses
// final = class cannot be override by other classes 
// abstract = cannot be used to create objects from an abstract class,need to inherit abstract class to use

/* variable modifier */
// final = declared variable or methods cannot be override
// static = fixed for the class,cannot used outside
// abstract = can used in an abstract class and abstract methods,
// dont have body(need to create class <new class name> extends <abstract class name>) 
// transient = skip attributes and methos when serializing
// synchronized = methods can be use only by one thread at same time
// volatile = value not cached thread-locally, always read from the "main memory"

/* Encapsulation - private modifier */
public class Person {
    // restricted access variable
	private String name;
}

/* get method */
public String getName() {
	// read restricted variable and return to public by using getName(),value read-only
	return name;
}

/* set method */
public void setName(String newName) {
	// write new variable to restricted variable,value can get by setName(),value write-only
	this.name = newName;
}
```

### Java Packages and API
```java
/* Reference library packages */
import package.name.Class;	// import single class
import java.util.Scanner;
import package.name.*;		// import whole package
import java.util.*;

/* structure direction of package */
// _____>root		--> root folder ie. java
//		_____>mypack		--> package folder ie. util
// 			_____>MyPackageClass.java	--> class folder ie.Scanner

// output	--> import root.mypack.MyPackageClass

/* package keyword */
// declare package name(must in lower case)
package com.testpackage.mypack;

// declare class name
class MyPackageClass {
	public static void main(String[] args) {
		code statements;
	}
}  
```

### Java Inheritance (Java 续承)
```java
/*sublass(子类/child)			superclass(父类/parent) */
(public/default) class class_name extends extend_class { 
	code statements; 
}

public class this_class.java extends new_class { 
	... 
} 

// superclass(create new parent class)
class Vehicle {
	protected String brand = "Ford";
	public void honk() {
		System.out.println("honk honk");
	}
}

// subclass(inherit own class.java from superclass)
class hellotest extends Vehicle {		
	private String modelName = "Mustang";
	public void main(String[] args) {
		hellotest myCar = new hellotest();	// create object
		myCar.honk();
		System.out.println(myCar.brand + " " + myCar.modelName):
	}
}
```

### Java Polmorphism (Java 多态) 
```java
/* 1 superclass being used by many subclasses */

class Animal {					// superclass
	public void animalSound() {
		System.out.println("Animal sound");
	}
}

class Pig extends Animal {		// subclass 1
	public void animalSound() {
		System.out.println("Pig sound");
	}
}

class Dog extends Animal {		// subclass 2
	public void animalSound() {
		System.out.println("Dog sound");
	}
}

class hellotest {					// main class
	public static void main(String[] args ) {
		Animal myAnimal = new Animal();		// declare object
		Animal myPig = new Pig();			// declare object
		Animal myDog = new Dog();			// declare object
		myAnimal.animalSound();				// execute
		myPig.animalSound();				// execute
		myDog.animalSound();				// execute
	}
}
```

### Java Inner Class/Nested Class (Java 嵌套类)
* to access inner class, need to create an outer class, then access inner class through outer class

```java
/*declare inner class */
OuterClass{			// outer layer part 
	// code statement
	// nested layer inner class
	InnerClass{
	// code statement
	}		
}

/* for loop structure example(nested loop) */
for(...) {			// outer layer
	for(...) {		// inner layer
	}	
}

/*to run */
public class hellotest {
	// declare object for outer class
	OuterClass myOuter = new OuterClass();
	// declare object for inner class
	OuterClass.InnerClass myInner = myOuter.InnerClass();
    // output object
	System.out.println(myInner.myInnerMethod());

	class OuterClass {
		int x = 10;
		class InnerClass {
			public int myInnerMethod() {
			return x;
		}
	}
}

public class hellotest {
	public static void main(String[] args) {
		OuterClass myOuter = new OuterClass();
		OuterClass.InnerClass myInner = myOuter.InnerClass();
		System.out.println(myInner.myInnerMethod());
	}
}
```

### Java Abstract (Java 抽象类)
* to improve security by hiding certain details and show only important details by using abstract 

```java
/* Classes and Methods */
// restricted class
abstract class Animal {
	public abstract void animalSound();
	public void sleep() {
		System.out.println("sleep");
	}
}

// inherit restricted class using extends
class Pig extends Animal {		
	public void animalSound() {
		System.out.println("Pig sound");
	}
}

//main class execute abstract class using inherited class name
class hellotest {					
	public static void main(String[] args) {
		// create object using inherited class 
		Pig myPig = new Pig();		
		myPig.animalSound();
		myPig.sleep();
	}
}
```

### Java Interface (Java 接口)
```java
// dont like abstract class,interface dont have body
interface Animal {
	// cannot define structure for interface class function,will throw error
	public void animalSound();
	public void sleep() ;
}

// use implements keyword to create body for interface class
class Pig implements Animal {
	public void animalSound() {
		System.out.println("Pig sound");
	}
	
	public void sleep() {
		System.out.println("sleep");
	}
}

// execute implemented class into main class
class hellotest {
	public static void main(String[] args) {
		Pig myPig = new Pig();
		myPig.animalSound();
		myPig.sleep();
	}
}

interface FirstInterface {
	public void myMethod();
}

interface SecondInterface {
	public void oOtherMethod();
}

// interface class can be implement in many interfaces class in one time, to create structure in one class 

class testClass implements FirstInterface,SecondInterface {
	public void myMethod() {			// interface 1 method
		System.out.println("first sound");
	}

	public void oOtherMethod() {		// interface 2 method
		System.out.println("second sound");
	}
}

class hellotest {
	public static void main(String[] args) {
		testClass myTest = new testClass();
		myTest.myMethod();
		myTest.oOtherMethod();
	}
}
```

### Java Enums 
* enum = special "class"(variable unchangeable like final variable),
* usually use for to values/variables that not going to change for future, 
* use pointer to point the variables in other class ( LEVEL.MEDIUM),
* cannot use to create object,but can implement for interfaces -->

```java
enum LEVEL {
	LOW,MEDIUM,HIGH
}

public class hellotest {
	public static void main(String[] args) {
		LEVEL myVar = LEVEL.MEDIUM;			// declare variable
		
		switch(myVar) {				// switch between LEVEL variable
			case LOW:
				System.out.println("Low level");
				break;
			case MEDIUM:
				System.out.println("Medium level");
				break;
			case HIGH:
				System.out.println("High level");
				break;
			}
	}
}

public class hellotest {
	public static void main(String[] args) {
		// loop through LEVEL variables
		for(LEVEL myVar : LEVEL.values()) {
			System.out.println(myVar);
		}
	}
}
```

### Java DateTime 
```java
/* Reference Library */
import java.time.*;

/*classes*/ 
//LocalDate = yyyy-MM-dd
//LocalTime = HH-mm-ss-ns
//LocalDateTime = yyyy-MM-dd-HH-mm-ss-ns
//DateTimeFormatter = display and parse date-time objects

/*date time formatter(.ofPattern("values") */
//yyyy-MM-dd = 1920-12-31
//dd/MM/yyyy = 31/12/2020
//dd-MMM-yyyy = 31-Dis-1920
//E,MMM dd yyyy = Thu, Dis 31 1920

//import localdatetime class
import java.time.LocalDateTime;
// import datetimeformatter
import java.time.format.DateTimeFormatter;

public class hellotest {
	public static void main(String[] args) {
		// declare object for current date time
		LocalDateTime myDateObj = LocalDateTime.now();
		System.out.println("Before change " + myDateObj);
		// declare format
		DateTimeFormatter myFormatObj = DateTimeFormatter.ofPattern("dd-MMM-yyyy");
		// convert to string
		String formattedDate = myDateObj.format(myFormatObj);
        // output string
		System.out.println("After change " + formattedDate);
	}
}
```

### Java List 
```java
/*ArrayList */
//Reference packages
// add(),get(),set(),remove(),clear(),size()
import java.util.ArrayList;
// sort()
import java.util.Collections;

/* syntax */
// declare arraylist as object
ArrayList<datatype> variable_name = new ArrayList<datatype>();
// declare raw type
ArrayList variable_name = new ArrayList();
//arraylist(no datatype,can store multiple items)

// add items to arraylist
variable_name.add("values1");					
	variable_name.add("values2");
	variable_name.add("values3");
	variable_name.add("values4");
	// get arr_position value
	variable_name.get(arr_position);
	// set arr_position with new value
	variable_name.set(arr_position, new_value);	
    // remove arr_position value
	variable_name.remove(arr_position);
	// clear all array elements
	variable_name.clear();
    // to determine the actual array size
	variable_name.size();
	// sort value in ascending order
	Collections.sort(variable_name);

import java.util.ArrayList;
import java.util.Collections;

public class hellotest {
	public static void main(String[] args) {
		// declare arraylist object
		ArrayList<String> cars = new ArrayList<String>();
		cars.add("Volvo");
		cars.add("BMW");
		cars.add("Ford");
		cars.add("Mazda");
		
		// loop through arraylist
		for(int i = 0; i < cars.size(); i++) {
			System.out.println(cars.get(i));
		}
		// sort arraylist
		Collections.sort(cars);
			for (String i : cars) {
				System.out.println(i);
			}
	}
}

/* Linked List */
// Reference packages
import java.util.LinkedList;
import java.util.Collections;

/* Syntax */
// declare linked list
LinkedList<dataype> variable_name = new LinkedList<datatype>();
// add value to first element
variable_name.addFirst();
// add value to last element
variable_name.addLast();
// get value for (index) element
variable_name.get(index);
// get value from first element
variable_name.getFirst();
// get value from last element
variable_name.getLast();
// remove first element value
variable_name.removeFirst();
// remove last element value
variable_name.removeLast();

import java.util.LinkedList;
import java.util.Collections;

public class hellotest {
	public static void main(String[] args) {
		LinkedList<String> products = new LinkedList<String>();
		String p1 = new String("Volvo");
		String p2 = new String("BMW");
		String p3 = new String("Ford");
		String p4 = new String("Mazda");
		products.add(p1);
		products.add(p2);
		products.add(p3);
		products.add(p4);
		String p5 = new String("Benz");
		products.addLast(p5);
			for(int i = 0; i < products.size(); i++) {
				System.out.println(products.get(i));
			}
		System.out.println("**********");
		System.out.println("The first product is : "+ products.getFirst());
		System.out.println("The last product is : " + products.getLast());
		
		products.removeLast();
		System.out.println("After deleted the product remaining : ");
			for( int i = 0; i < products.size(); i ++) {
				System.out.print(products.get(i) + "\t");
			}
		System.out.println("\n**********");
		
		Collections.sort(products);
			for (String i : products) {
				System.out.println(i);
			}
		}
}
```

### Java Map(HashMap and TreeMap)
##### HashMap
* HashMap is element with pair of key + value, key is unique, value can be same
```java
// Reference packages
// Hashmap package
import java.util.HashMap;

/* Syntax */
HashMap<datatype> variable_name = new HashMap<datatype>();
	// clear all key-value
	variable_name.clear();
	// find Map object value
	 variable_name.containsKey(Object value);
	 // return object value
	variable_name.get(Object key);
	// add key-value to Map,if key exists, replace old key-value
	variable_name.put("key","value");
	// copy other Map to selected Map
	variable_name.putAll(Map);
	// selected key-value,if not exist,return null
	variable_name.remove(Object key);
	// Java 8 new delete key-value method
	variable_name.remove(Object key, Object value);
	// return all Map key-value to a Set
	variable_name.entrySet();
	// return Map key
	variable_name.keySet();
	// check Map is empty(no key-value), if empty return true
	variable_name.isEmpty();
	// return size of Map
	variable_name.size();
	// return Map values
	variable_name.values();

import java.util.HashMap;
import java.util.Iterator;
import java.util.Scanner;

public class hellotest {
	public static void main(String[] args) {
		HashMap users = new HashMap();
		users.put("11", "User1");
		users.put("22", "User2");
		users.put("33", "User3");
		users.put("44", "User4");
		users.put("55", "User5");
		System.out.println("**********");
		
		Iterator it = users.keySet().iterator();
			while(it.hasNext()) {
				Object key = it.next();
				Object val = users.get(key);
				System.out.println("User ID : " + key + " User Name : " + val);
			}
		
		Scanner input = new Scanner(System.in);
		System.out.println("Please input deleted ID : ");
		int num = input.nextInt();
		
		if(users.containsKey(String.valueOf(num))) {
			users.remove(String.valueOf(num));
		}
		else {
			System.out.println("This user is not exists! ");
		}
		
		System.out.println("*****Users List*****");
		it = users.keySet().iterator();
			while(it.hasNext()) {
				Object key = it.next();
				Object val = users.get(key);
				System.out.println("User ID : " + key + " User Name : " + val);
			}
		}
}
```

### Java Sets(HashSet and TreeSet) 
1. HashSet 
* items is Sets is unique and wont appears twice although have same items
```java
// Reference packages
import java.util.HashSet;

/* Syntax */
HashSet<datatype> variable_name = new HashSet<datatype>();

import java.util.HashSet;

public class hellotest {
	public static void main(String[] args) {
		HashSet<Integer> numbers = new HashSet<Integer>();
		numbers.add(4);
		numbers.add(7);
		numbers.add(8);
		
		for(int i = 1; i <= 10; i++) {
			if(numbers.contains(i)) {
				System.out.println(i + " was found in the set.");
			}
			else {
				System.out.println(i + " was not found is the set.");
			}
		}
	}
}

import java.util.HashSet;
import java.util.Iterator;

public class hellotest {
	public static void main(String[] args) {
		HashSet<String> courseSet = new HashSet<String>();
		String course1 = new String("Java");
		String course2 = new String("Python");
		String course3 = new String("HTML");
		String course4 = new String("PHP");
		courseSet.add(course1);
		courseSet.add(course2);
		courseSet.add(course3);
		courseSet.add(course4);
		System.out.println("All courses : ");
		
		Iterator<String> it = courseSet.iterator();
			while(it.hasNext()) {
				System.out.println(" <" + (String)it.next() + "> ");
			}
		System.out.println("There are " + courseSet.size() + " course.");
	}
}
```

2. TreeSet
* TreeSet different with HashSet is becuase have SortedSet interface,
* can implement using SortedSet to sort value in ASCENDING ORDER, only can arrange and compare with same object type
```java
// Reference packages
import java.util.TreeSet;
import java.util.SortedSet;

/* Syntax */
// return first set element
variable_name.first();
//SortedSet
variable_name.headSet();
// return last set element
variable_name.last();
//SortedSet
variable_name.tailSet();

import java.util.TreeSet;
import java.util.Iterator;
import java.util.Scanner;
import java.util.SortedSet;

public class hellotest {
	public static void main(String[] args) {
		TreeSet<Double> scores = new TreeSet<Double>();
		Scanner input = new Scanner(System.in);
		System.out.println("********* Student Result System *********");
			for(int i =0; i < 5; i++) {
				System.out.println("No: " + (i + 1) + " student's result : ");
				double score = input.nextDouble();
				scores.add(Double.valueOf(score));
			}
		
		Iterator<Double> it = scores.iterator();
		System.out.println("Student result in ascending order: ");
			while(it.hasNext()) {
				System.out.print(it.next() + "\t");
			}
			
		System.out.println("\nPlease input searching result: ");
		double searchScore = input.nextDouble();
			if(scores.contains(searchScore)) {
				System.out.println("The result's: " + searchScore + " student is exists! ");
			}
			else {
			System.out.println("The result's: " + searchScore + " students is not exists.");
			}
		
		SortedSet<Double> score1 = scores.headSet(60.0);
		System.out.println("\nFailed results are: ");
			for(int i = 0; i< score1.toArray().length; i++) {
				System.out.print(score1.toArray()[i] + "\t");
			}
		SortedSet<Double> score2 = scores.tailSet(90.0);
		System.out.println("\n90% and above score are: ");
			for(int i = 0; i < score2.toArray().length; i++) {
				System.out.print(score2.toArray()[i] + "\t");
			}
	}
}
```

### Java Iterator (Java 迭代器)
* use iterator to loop through collection,such as ArrayList and HashSet
```java
// Reference packages
import java.util.Iterator;
import java.util.Collection;

/* Syntax */
Iterator<datatype> it(variable_name) = arrObj.iterator();
variable_name.next(); 
variable_name.hasNext();
// remove targeted element
variable_name.remove();
variable_name.forEachRemaining();

import java.util.HashSet;
import java.util.Iterator;
import java.util.Collection;

public class hellotest {
	public static void main(String[] args) {
		Collection objs = new HashSet();
		objs.add("Java");
		objs.add("HTML");
		objs.add("PHP");
		
		Iterator it= objs.iterator();
			while(it.hasNext()) {
			String obj = (String) it.next();
			System.out.println(obj);
				if(obj.contentEquals("HTML")) {
					it.remove();
				}
			obj = "Python";
			}
		System.out.println(objs);
	}
}
```

### Java Wrapper Classes(Java 包装类)
* use for working with objects declaration such as ArrayList
```java
/* Keywords */
// byte,byteValue()
Byte
//short,shortValue()
Short
// int,intValue()
Integer
//long,longValue()
Long
// float,floatValue()
Float
// double,doubleValue()
Double
// boolean,booleanValue()
Boolean
// char,charValue()
Character
// convert objects to string(Integet to String)
varName.toString();
// equals to ( == )
obj.equals(Object o);
// return class name
obj.getClass().getName();
// get parent class name
obj.getClass().getSuperClass().getName();
obj.getClass().getInterfaces()[i]
```

### Java Exceptions (try...catch)
* use for debugging the program and troubleshoot errors for the code, and for other code statement purpose
```java
try {
	//code need to try
}catch (Exception e) {
	// output exception type
	e.printStackTrace();
	//block of code to handel error(error message)
}
finally {
	//code to execute after try...catch(message after error code) 
}
throw new (/*Exception type*/) ("text here");

/* exception type */
//ArithmeticException(Access denied,access granted)
//FileNotFoundException
//ArrayIndexOutOfBoundsException
//SecurityException
```

### Java Regular Expression (Java 正则表达式)
* can use to perform text search and text replace operations
```java
// Reference packages
import java.util.regex.*;
import java.util.regex.Pattern;
import java.util.regex.Matcher;
import java.util.regex.PatternSyntaxException;

import java.util.regex.Matcher;
import java.util.regex.Pattern;
/* Range of expression to find(Pattern.compile("Expression",Flag) */
// find 1 character between bracket
[abc]
// find 1 character not between bracket
[^abc]
// find 1 character from range 0 to 9
[0-9]
// find a | b
|
// just one instance of any character
.
// find a match beginning of a string as in : ^Hello
^
// find a match at the end of string as in : World$
$
// find a digit
\d
// find a whitespace character
\s
// find a word like \bWORD or WORD\b
\b
// find the Unicode character with hexadecimal number xxxx
\\uxxxx
// quantifiers define quantities to match
n+,n*,n?,n{x},n{x,y},n{x,}

public class hellotest {
	public static void main(String[] args) {
// pattern need to find,pattern flag(CASE_INSENSITIVE,LITERAL,UNICODE_CASE)
		Pattern pattern = Pattern.compile("patternTxt", Pattern.CASE_INSENSITIVE);
		// text need to match with pattern
		Matcher matcher = pattern.matcher("Match the patternTxt.");	
		// find through matcher
		boolean matchFound = matcher.find();
		if(matchFound) {
			// if true, throw code
			System.out.println("Match found");
		}else {
			// if false, throw code
			System.out.println("Match not found");
		}
	}
}
```


### Java Threads (Java 多线程)
* Thread life cycle
![Thread Life Cycle](https://www.runoob.com/wp-content/uploads/2014/01/java-thread.jpg) 

```java
/* Thread Priority */
// Range from 1 - 10
// Thread.MIN_PRIORITY(1) - Thread.NORM_PRIORITY(5) - 10 Thread.MAX_PRIORITY(10)

/* Creating thread */
public class class_name implements Runnable {}
public class class_name extends Thread {}
public class class_name implements Callable {}

// class extends thread
public class hellotest extends Thread {
	public static int amount = 0;
	
	public static void main(String[] args) {
		// create object
		hellotest thread = new hellotest();
		// start thread
		thread.start();
		// check thread is still alive
		while(thread.isAlive()) {
			System.out.println("Waiting...");
		}
		System.out.println("Main: " + amount);
		amount++;
		System.out.println("Main: " + amount);
	}

	public void run() {
		amount++;
	}
}

/* hellotest.java */
public class hellotest extends Thread {
	private int number; 
	public hellotest(int number) {
		this.number = number;
	}
	
	public void run() {
		int counter = 0;
		int guess = 0;
		do {
			guess = (int) (Math.random() * 100 + 1);
			System.out.println(this.getName() + " guesses " + guess);
			counter++;
		}while( guess != number);
		
		System.out.println("** Correct! " + this.getName() + " in " + counter + " guesses.**");
	}
}

/* OtherClass.java */
public class OtherClass implements Runnable {
	private String message;
	
	public OtherClass(String message) {
			this.message = message;
	}

	public void run() {
		while(true) {
			System.out.println(message);
		}
	}
}

/* ThreadClass.java */
public class ThreadClass {
	public static void main(String[] args) {
		Runnable hello = new OtherClass("Hello");
		Thread thread1 = new Thread(hello);
		thread1.setDaemon(true);
		thread1.setName("hello");
		System.out.println("Starting hello thread...");
		
		Runnable bye = new OtherClass("Goodbye");
		Thread thread2 = new Thread(bye);
		thread2.setPriority(Thread.MIN_PRIORITY);
		thread2.setDaemon(true);
		System.out.println("Starting goodbye thread...");
		thread2.start();
		
		System.out.println("Starting thread3...");
		Thread thread3 = new hellotest(27);
		thread3.start();
		try {
			thread3.join();
		}catch(InterruptedException e) {
			System.out.println("Thread interrupted.");
		}
		
		System.out.println("Starting thread4...");
		Thread thread4 = new hellotest(75);
		thread4.start();
		System.out.println("main() is ending...");
	}
}
```

### Java Lambda Expression
* supported by amy languages, c++,c#,Java,Python,Javascript,use to shorten the time to write code

```java
/* Syntax Lambda */
(parameter) -> {
	Lambda code 
}
result = (int a,int b) -> {return a + b}; 

/* OtherClass.java */
public interface OtherClass {
	int calculateInt(int a, int b);
}

/* hellotest.java */
public class hellotest {
	public static OtherClass calculate(char opr) {
		OtherClass result;
		if(opr == '+') {
			// Regular Expression(result = new OtherClass() {public int calculateInt(int a, int b) {}
			result = (int a, int b) -> {
				return a + b;
            };
		} else {
			// Regular Expression(result = new OtherClass() {public int calculateInt(int a, int b) {}
			result = (int a, int b) -> {
				return a - b;
			};
		}
		return result;
	}

	public static void main(String[] args) {
		int n1 = 10;
		int n2 = 5;
		
		OtherClass f1 = calculate('+');
		OtherClass f2 = calculate('-');
		System.out.println(n1 + " + " + n2 + " = " + f1.calculateInt(n1, n2));
		System.out.println(n1 + " - " + n2 + " = " + f1.calculateInt(n1, n2));
	}
}
```

### Java File Stream
```java
import java.io.*;

public class hellotest {
	public static void main(String args[]) {
		try {
			byte[] bWrite = { 11, 21, 3, 40, 5 };
			OutputStream os = new FileOutputStream("D:\\Temp\\AOI+AXI\\newfile.bar");
				for(int x = 0; x < bWrite.length; x++) {
					os.write(bWrite[x]);
				}
				os.close();
				
				InputStream is = new FileInputStream("D:\\Temp\\AOI+AXI\\newfile.bar");
				int size = is.available();
					for(int i = 0; i < size; i++) {
						System.out.print((char) is.read() + " ");
					}
					is.close();
		}catch (IOException e) {
			System.out.print("Exception");
		}
	}
}
```
