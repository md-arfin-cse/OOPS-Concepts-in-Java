# OOPS-Concepts-in-Java

OOPs concepts in Java | What is OOPs in Java?
By Great Learning Team -Jan 2, 2021126398 0
 Share
In this blog, we are going to learn about the basics of OOPs concepts in java. Object-oriented programming is a model that provides different types of concepts, such as inheritance, abstraction, polymorphism, etc. These concepts aim to implement real-world entities in programs. They create working methods and variables to reuse them without compromising security. This emphasizes data rather than functions. Many of the most widely used and significant object-oriented programming languages include Java, C++, C#, JavaScript, Python, Ruby, Perl, Smalltalk etc.

If you want to deep dive further, do check out our Software Engineering Courses at Great Learning in collaboration with top engineering colleges and universities, including IIT Madras, Great Lakes, Jain University, & IIIT Hyderabad. Participate in regularly organized career accelerated programs and placement drives offered by Great Learning and get hired by the top leading companies across different industries.

What is OOPs?
What are Objects?
What are Classes?
What is Abstraction?
What is Inheritance?
What is Polymorphism?
What is Encapsulation?
Coupling in Java
Cohesion in Java
Association in Java
Aggregation
Composition in Java
Methods in Java
Static Method in Java
Abstract Method in Java
Final Method in Java
Equals Method in Java
Message Passing in Java
Can Polymorphism, Encapsulation and Inheritance work together?
Advantages of OOPs Concept
Disadvantages of OOPs Concept
Differences between Object-Oriented Programming, Procedural Oriented Programming, Structured Programming?
Summary
FAQ
What is OOPs?
Object-oriented programming is a method used for designing a program using classes and objects. Object-oriented programming is also called the core of java. Object-oriented programming organizes a program around objects and well-defined interfaces. This can also be characterized as data controlling for accessing the code. In this type of approach, programmers define the data type of a data structure and the operations that are applied to the data structure. This implies software development and maintenance by using some of the concepts:

Object 
Class
Abstraction
Inheritance 
Polymorphism
Encapsulation
What are the Concept of oops in JAVA ?
What is OOPs concepts in java? 
OOps, concepts in java is to improve code readability and reusability by defining a Java program efficiently. The main principles of object-oriented programming are abstraction, encapsulation, inheritance, and polymorphism. These concepts aim to implement real-world entities in programs.

What are Objects?  
Objects are always called as instances of a class. Objects are created from class in java or any other languages. Objects are those that have state and behaviour. Objects are abstract data types (i.e., objects behaviour is defined by a set of values and operations).

These objects always correspond to things found in the real world, i.e., real entities. So, they are also called a run time entity of the world. These are self–contained which consists of methods and properties which makes data useful. Objects can be both physical and logical data. It contains addresses and takes up some space in memory. Some of the examples of objects are a dog, chair, tree etc. 

When we treat animals as objects, it has states like colour, name, breed etc., and behaviours such as eating, wagging the tail etc.

Suppose, we have created a class called My book, we specify the class name followed by the object name, and we use the keyword new.

Example 1:

1
2
3
4
5
6
7
Public class Mybook {
int x=10;
Public static void main (String args []) {
Mybook Myobj= new Mybook ();
System.out.println(MyObj.x);
}
}
In the above example, a new object is created, and it returns the value of x which may be the number of books.

Mybook Myobj= new Mybook ();

 This is the statement used for creating objects.

System.out.println(Myobj.x);

This statement is used to return the value of x of an object.

We can also create multiple objects in the same class and we can create in one class and access it in another class. This method is used for better organization of classes and always remember that name of the java file and the class name remains the same. 

Example 2:

The below example shows how multiple objects are created in the same class and how they are accessed from another class.

Mybook.java
1
2
3
4
Public class Mybook {
int x=10;
int y=8;
}
Count.java
1
2
3
4
5
6
7
8
9
Class Count {
Public static void main (String [] args)
{
Mybook myobj1 = new myobj1();
          Mybook myobj2 = new myobj2();
           System.out.println (myobj1.x);
System.out.println (myobj2.y);
}
}
When this program is compiled, it gives the result as 10, 8 respectively.

What are Classes?
Classes are like object constructors for creating objects. The collection of objects is said to be a class. Classes are said to be logical quantities. Classes don’t consume any space in the memory. Class is also called a template of an object. Classes have members which can be fields, methods and constructors. A class has both static and instance initializers.

A class declaration consists of:

Modifiers:Can be public or default access.
Class name: Initial letter.
Superclass: A class can only extend (subclass) one parent.
Interfaces: A class can implement more than one interface.
Body: Body surrounded by braces, { }.
A class keyword is used to create a class. A simplified general form of the class definition is given below:

1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
class classname {
type instance variable 1;
type instance variable 2;
.
.
.
type instance variable n;
type methodname 1 (parameter list) {
// body od method 
}
type methodname 2 (parameter list) {
// body od method 
}
type methodnamen (parameter list) {
// body od method 
}
 }
The variables or data defined within a class are called as instance variables. Code is always contained in the methods. Therefore, the methods and variables defined within a class are called members of the class. All the methods have the same form as main () these methods are not specified as static or public. 

What is Abstraction?  
Abstraction is a process which displays only the information needed and hides the unnecessary information. We can say that the main purpose of abstraction is data hiding. Abstraction means selecting data from a large number of data to show the information needed, which helps in reducing programming complexity and efforts.  

There are also abstract class and abstract methods. An abstract class is a type of class that declares one or more abstract methods. An abstract method is a method that has a method definition but not implementation. Once we have modelled our object using data abstraction, the same sets of data can also be used in different applications—abstract classes, generic types of behaviours and object-oriented programming hierarchy. Abstract methods are used when two or more subclasses do the same task in different ways and through different implementations. An abstract class can have both the methods, i.e., abstract methods and regular methods.

Now let us see an example related to abstraction.

Suppose we want to create a student application and ask to collect the information about the student.

We collect the following information.  

Name 
Class
Address
Dob
Fathers name
Mothers name and so on. 
We may not require every information that we have collected to fill the application. So, we select the data that is required to fill the application. Hence, we have fetched, removed, and selected the data, the student information from large data. This process is known as abstraction in oops concept.

Abstract class example:

1
2
3
4
5
6
7
8
9
10
11
12
13
14
//abstract parent class 
        Abstract class animal {
         //abstract method 
      public abstract void sound ( ) ;
         }
     Public class lion extends animal {
      Public void sound ( ) {
System.out.println (“ roar “ );
}
public Static void main ( String args [ ] ) {
 animal obj = new lion ( );
obj. sound ();
}
}
Output: 
Roar

What is Inheritance?
Inheritance is a method in which one object acquires/inherits another object’s properties, and inheritance also supports hierarchical classification. The idea behind this is that we can create new classes built on existing classes, i.e., when you inherit from an existing class, we can reuse methods and fields of the parent class. Inheritance represents the parent-child relationship.

For example, a whale is a part of the classification of marine animals, which is part of class mammal, which is under that class of animal. We use hierarchical classification, i.e., top-down classification. If we want to describe a more specific class of animals such as mammals, they would have more specific attributes such as teeth; cold-blooded, warm-blooded, etc. This comes under the subclass of animals where animals come under superclass. The subclass is a class which inherits properties of the superclass. This is also called a derived class. A superclass is a base class or parental class from which subclass inherits properties.

We use inheritance mainly for method overriding and R:

To inherit a class, we use the extend keyword. 


There are five types of inheritance single, multilevel, multiple, hybrid and hierarchical. 

Single level  
In this one class i.e., derived class inherits properties from its parental class.  This enables code reusability and also adds new features to the code. Example: class b inherits properties from class a.

Class A is base or parental class and class b is derived class.

Syntax: 

1
2
3
4
5
6
Class a {
…
}
Class b extends class a {
…
}
Multilevel
This one class is derived from another class which is also derived from another class i.e., this class has more than one parental class, hence it is called multilevel inheritance.

Syntax:

1
2
3
4
5
6
7
8
9
Class a {
….
}
Class b extends class a {
….
}
Class c extends class b {
… 
}
Hierarchical level 
In this one parental class has two or more derived classes or we can say that two or more child classes has one parental class.

Syntax:

1
2
3
4
5
6
7
8
9
Class a {
…
}   
Class b extends class a {
..
}
Class c extends class a {
..
}
Hybrid inheritance
This is the combination of multiple and multilevel inheritance and in java multiple inheritance is not supported as it leads to ambiguity and this type of inheritance can only be achieved through interfaces.

Consider that class a is the parental or base class of class b and class c and in turn class b and class c are parental or base class of class d. Class b and class c are derived classes from class a and class d is derived class from class b and class c.

Following program creates a super class called add and a subclass called sub, uses extend keyword to create a subclass add.

1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
// a simple example of inheritance 
//create a superclass
Class Add {
int my;
int by;
void setmyby (int xy, int hy) {
my=xy;
by=hy;
}
}
/create a sub class
class b extends add {
int total;
void sum () {
public Static void main (String args [ ] ) {
b subOb= new b ( );
subOb. Setmyby (10, 12);
subOb. Sum ( ) ;
System.out.println(“total =” + subOb. Total);
}
} 
It gives output as – total = 22

What is Polymorphism?
Polymorphism refers to many forms, or it is a process that performs a single action in different ways. It occurs when we have many classes related to each other by inheritance. Polymorphism is of two different types, i.e., compile-time polymorphism and runtime polymorphism. One of the examples in Compile time polymorphism is that when we overload a static method in java. Run time polymorphism is also called a dynamic method dispatch is a method in which a call to an overridden method is resolved at run time rather than compile time. In this method, the overridden method is always called through the reference variable. By using method overloading and method overriding, we can perform polymorphism. Generally, the concept of polymorphism is often expressed as one interface, multiple methods. This reduces complexity by allowing the same interface to be used as a general class of action. 

Example:

1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
public class Bird {
…
Public void sound ( ) {
System.out.println ( “ birds sounds “ );
}
}
public class pigeon extends Bird {
…
@override
public void sound ( ) {
System.out.println( “ cooing ” ) ;
}
}
public class sparrow extends Bird ( ) {
….
@override
Public void sound ( ){
System.out.println( “ chip ” ) ;
}
}
In the above example, we can see common action sound () but there are different ways to do the same action. This is one of the examples which shows polymorphism.

Polymorphism in java can be classified into two types:

Static / Compile-Time Polymorphism
Dynamic / Runtime Polymorphism
What is Compile-Time Polymorphism in Java?
Compile-Time polymorphism in java is also known as Static Polymorphism. to resolved at compile-time which is achieved through Method Overloading.

What is Runtime Polymorphism in Java?
Runtime polymorphism in java is also known as Dynamic Binding which is used to call to an overridden method that is resolved dynamically at runtime rather than at compile-time. 

What is Encapsulation?
Encapsulation is one of the concepts in OOPs concepts; it is the process that binds together the data and code into a single unit and keeps both from being safe from outside interference and misuse. In this process, the data is hidden from other classes and can be accessed only through the current class’s methods. Hence, it is also known as data hiding. Encapsulation acts as a protective wrapper that prevents the code and data from being accessed by outsiders. These are controlled through a well-defined interface. 

Encapsulation is achieved by declaring the variables as private and providing public setter and getter methods to modify and view the variable values. In encapsulation, the fields of a class are made read-only or write-only. This method also improves the re-usability. Encapsulated code is also easy to test for unit testing.

Example:

1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
22
class animal {
// private field 
private int age;
//getter method 
Public int getage ( ) {
return age;
}
//setter method 
public void setAge ( int age ) {
this. Age = age;
}
}
class Main {
public static void main (String args []);
//create an object of person 
Animal a1= new Animal ();
//change age using setter 
A1. setAge (12);
// access age using getter 
System.out.println(“ animal age is ” + a1. getage ( ) );
}
}
Output: Animal age is 12

In this example, we declared a private field called age that cannot be accessed outside of the class.

To access age, we used public methods. These methods are called getter and setter methods. Making age private allows us to restrict unauthorized access from outside the class. Hence this is called data hiding. 

Coupling in Java
Coupling refers to the relationship between two classes. It indicates the knowledge one object or class has of another. That means that if one class changes its properties or behavior, it will affect the dependent changes in the other class. Therefore, these changes will depend upon the level of interdependence the two classes have between them. There are two types of coupling, namely tight coupling, and loose coupling.

Tight coupling: If one class is strongly interrelated to another class, it is said to have tight coupling with that class. 
public class College{
public void status() {
System.out.println("College is open today");
}
}
public class Student{
College obj = new College();
public void goToCollege() {
obj.status();
}
}
In the above code example, the student class is dependent on the college class. That is, any change in the college class requires student class to change. Here, therefore, student class and college class are tightly coupled with each other.

Loose coupling: If one class is weakly interrelated to another class, it is said to have loose coupling with that class. Loose coupling is preferred over tight coupling. A class can achieve this with the help of interfaces, as shown below. 
public interface College{
void status();
}
class CollegeStatus1 implements College{
public void status() {
System.out.println("College is open monday to friday");
}
}
class CollegeStatus2 implements College{
public void status() {
System.out.println("College is open on saturday");
}
}
public class Student{
College obj = new CollegeStatus1();
public void goToCollege() {
obj.status();
}
}
In the above code example, CollegeStatus1 and CollegeStatus2 are loosely coupled. Here, student class is not directly or tightly coupled with a CollegeStatus1 or CollegeStatus2 class. By applying a dependency injection mechanism, the loose coupling implementation is achieved to allow a student to go to college with any class which has implemented a college interface. In addition, it means we can use CollegeStatus2 whenever the college is open on Saturday.

Cohesion in Java
Cohesion measures how the methods and the attributes of a class are meaningfully and strongly related to each other and how focused they are in performing a single well-defined task for the system. Cohesion is used to indicate the degree to which a class has a single, well-focused responsibility. More cohesive classes are good to keep them for code reusability. Low cohesive classes are difficult to maintain as they have a less logical relationship between their methods and properties. It is always better to have highly cohesive classes to keep them well focused for a single work.

Low Cohesion: In the following code, we have a class called Book. But it is less cohesive because it comprises less focussed and independent attributes and methods to the class. This class should contain information related to the Book. Therefore, the person name and age method are making this classless cohesive.
class Book{
int price = 299; //related attribute
String name = "Sam"; //unrelated attribute
//related methods to Book class
public String author(String name) {
return name;
}
public String title(String subject) {
return subject;
}
public int id(int number) {
return number;
}
//unrelated methods to Book class
public int age(int age) {
return age;
}
}
High Cohesion: When the class has a single well-defined purpose or task, it is said to be highly cohesive. So, in the above example code, if we remove the information related to the person, then the class becomes highly cohesive, as shown below.
class Book{
int price = 299; //related attribute
//related methods to Book class
public String author(String name) {
return name;
}
public String title(String subject) {
return subject;
}
public int id(int number) {
return number;
}
}
Association in Java
Association is a relation between two separate classes that establishes with the help of their Objects. It specifies the relationship between two or more Objects. Association can be one-to-one, one-to-many, many-to-one, many-to-many. Let us understand this with real-world examples, suppose the relationship between the bus and the passengers. A bus can have only one driver(one-to-one). Many passengers can associate with the single bus(many-to-one). A single passenger can associate with many different buses(one-to-many). Also, many passengers can associate with the many different buses(many-to-many). One object is associated with another object to use the functionality and services provided by another object. 

Consider the following code below:

//class bus
class Bus
{
private String name;
// bus name
Bus(String name)
{
this.name = name;
}
public String getBusName()
{
return this.name;
}
}

//passenger class
class Passenger
{   
// passenger name
private String name;
// passenger seat id number
private int seatId;
Passenger(String name, int seatId)
{
this.name = name;
this.seatId = seatId;
}
public String getPassengerName()
{
return this.name;
}
public int getPassengerId()
{
return this.seatId;
}
}

//Association between both the
//classes in the main method
class Demo
{
public static void main (String[] args)
{
Bus bus = new Bus("Shree Travels");
        Passenger psg = new Passenger("Sneha", 52);
System.out.println(psg.getPassengerName() + " with seat number " + psg.getPassengerId()
+ " is a passenger of " + bus.getBusName());
}
}
Output:

Sneha with seat number 52 is a passenger of Shree Travels

Explanation:

In the above example, two separate classes Bus and Passenger, are associated through their Objects inside the class Demo. In this way, we can establish the relationship between two different classes by using the concept of association. A bus can have many passengers, So it is a one-to-many relationship.

Association is of two types, i.e., Aggregation and Composition.

Let’s discuss the two in detail.

Aggregation
Aggregation is a weak association. Aggregation represents a relationship between an object containing other objects. Aggregation is an association that represents a part of a whole relationship where a part can exist without a whole. Let’s take an example of the relationship between Group and Person. A Person may belong to multiple Groups. Hence a Group can have multiple Persons. But if we delete a Group, the Person object will not destroy. Aggregation represents the Has-A relationship. Aggregation is a unidirectional association, i.e., a one-way relationship. For instance, the group can have persons, but vice versa is not possible and thus unidirectional. In Aggregation, both the entries can survive individually, which means ending one entity will not affect the other entity. Hence, both objects are independent in aggregation.

Considering the following code example:

import java.util.*;

//person class
class Person
{
private String name;
private int age ;
Person(String name, int age)
{
this.name = name;
this.age = age;
}
public String getName() {
return name;
}
public int getAge() {
return age;
}
}

/* Group class contains the list of person
Objects. It is associated with the person
class through its Object(s). */

//group class
class Group
{
private String groupName;
private List<Person> persons;
Group(String groupName, List<Person> persons)
{
this.groupName = groupName;
this.persons = persons;
}
}

//main method
class Demo
{
public static void main (String[] args)
{   
//creating objects of person class
Person a = new Person("Tanmay", 17);
Person b = new Person("Sam", 18);
Person c = new Person("Pitu", 19);
Person d = new Person("Khushi", 20);
//making a list of persons belongs to social welfare group
List<Person> p1 = new ArrayList<>();
p1.add(a);
p1.add(c);
//making a list of persons belongs to drama fest group
List<Person> p2 = new ArrayList<>();
p2.add(b);
p2.add(d);
//creating objects of group class
Group swGrp = new Group("Social Welfare", p1);
Group dfGrp = new Group("Drama Fest", p2);
//before deleting drama fest group
System.out.println("List of persons in Drama Fest group:");
for(Person p : p2) {
System.out.println("Person name: " + p.getName() + ", Age:" + p.getAge() + ", Group: Drama Fest");
}
//deleting drama fest group
dfGrp = null;
//after deleting drama fest group
//person list will not destroy
System.out.println("List of persons after deleting Drama Fest group:");
for(Person p : p2) {
System.out.println("Person name: " + p.getName() + ", Age: " + p.getAge());
}
}
}
Output:

List of persons in Drama Fest group:

Person name: Sam, Age:18, Group: Drama Fest

Person name: Khushi, Age:20, Group: Drama Fest

List of persons after deleting Drama Fest group:

Person name: Sam, Age: 18

Person name: Khushi, Age: 20

Explanation:

Here, we can see that the two classes Person and Group, are associated with each other with the help of objects. There are two groups social welfare and drama fest. We created these groups by using the person class. The group has a list of persons. We have two persons Sam and Khushi, in the Drama Fest group as shown in the output. Afterward, we deleted this group by setting the instance of group equals to null. But, our list of persons remains undestroyed due to the weak association, i.e., aggregation, even after the group was deleted.

Composition in Java
Composition is a strong association. Composition is an association that represents a part of a whole relationship where a part cannot exist without a whole. Let’s take an example of the relationship between School and Room. The school object consists of several rooms. Whenever the school object destroys automatically, all the room objects will be destroyed, i.e., without the existing school object, there is no chance of an existing dependent object. So these are strongly associated, and this relationship is called composition. If a whole is deleted, then all parts are deleted. So composition represents the part-of relationship. 

Whenever there is a composition between two entities, the created object cannot exist without the other object. Thus, in composition, both entities are dependent on each other.

Consider the following code example:

import java.util.*;   
// activity room class
class ActivityRoom {  
    public String subject;   
    public int id;   
    
    ActivityRoom(String subject, int id)   
    {   
        this.subject = subject;   
        this.id = id;   
    }   
    
}   
// department class   
class Department {   
private String name;
    //list of activity rooms in a department.   
    private List<ActivityRoom> ar; 
    
    Department(List<ActivityRoom> ar)  
    {  
        this.ar = ar;  
    }   
    // Getting total number of colleges  
    public List<ActivityRoom> getActivityRoomsInDepartment()   
    {   
        return ar;   
    }   
}   
class Demo {   
    public static void main(String[] args)   
    {   
        // Creating the Objects of activity room class.   
     ActivityRoom a1 = new ActivityRoom("Technical", 601);   
     ActivityRoom a2 = new ActivityRoom("Business", 602);   
     ActivityRoom a3 = new ActivityRoom("Economics", 603);  
     
        // making the list of activity rooms.   
        List<ActivityRoom> act = new ArrayList<ActivityRoom>();   
        act.add(a1);   
        act.add(a2);   
        act.add(a3);  
        
        // Creating the Object of department class. 
        Department d = new Department(act); 
        
        // making the list of activity rooms in department.   
        List<ActivityRoom> arlist = d.getActivityRoomsInDepartment();   
        for (ActivityRoom a : arlist) {   
            System.out.println(a.subject + " activity room with id " + a.id);   
        }  
        
    }   
}
Output:

Technical activity room with id 601

Business activity room with id 602

Economics activity room with id 603

Explanation:

Here we have two classes Activity room and Department. A department composed of different subject activity rooms. So, If the department gets destroyed, then All activity rooms within that department will be destroyed, i.e., the activity room can not exist without the department. That’s why it is composition.

Methods in Java
A method in java is a block of code or collection of statements grouped together to complete a certain job or operation. A method is used to achieve the reusability of code. A method is written once and can be utilized many times. It also gives the easy modification and readability of code. A method is executed only when we call or invoke it. We have two categories of methods in java, i.e., pre-defined and user-defined. Predefined methods are the methods that are already defined in the Java class libraries. When the particular method is written by the user or programmer, it is known as a user-defined method. User-defined methods can be modified according to the requirement.

Let’s discuss:

Static method in Java
Abstract method in Java
Finalize method in Java
Equals method in Java
Static Method in Java
A method that has the static keyword in the declaration is known as the static method. In other words, a method that belongs to a class rather than an instance of a class is known as a static method. We can also create a static method by using the keyword static before the method name. The main benefit of a static method is that we can invoke the static method without even creating an object. It can access static data members and also change their values. It is used to create an instance method. It is invoked by using the class name. The main() method is a common example of the static method.

Example:

public class Demo  
{  
public static void main(String[] args)   
{  
displaymethod();  
}  
static void displaymethod()   
{  
System.out.println("It is an example of static method.");  
}  
}  
Output:

It is an example of a static method.

Abstract Method in Java
A method that is declared with keyword abstract is called an abstract method. The abstract method does not have an implementation or body, or block of code. The abstract method must always be declared in an abstract class, or we can say that if a class has an abstract method, it should be declared abstract. If a class has an abstract method, it should be declared abstract, but vice versa is not true, which means that an abstract class doesn’t need to have an abstract method compulsory. Also, If a normal class extends an abstract class, then the class must have to implement all the abstract parent class’s abstract methods, or it has to be declared abstract.

Example:

//abstract class area
abstract class Area{
 /* These two are abstract methods, the child class
  * must implement these methods
  */
 public abstract int areaSquare(int s);
 public abstract int areaRectangle(int l, int b);
 //Normal method 
 public void display(){
System.out.println("Normal method in abstract class Area");
 }
}
//Normal class extends the abstract class
class Demo extends Area{

 /* If we don't provide the implementation of these two methods, the
  * program will throw compilation error.
  */
 public int areaSquare(int s){
return s*s;
 }
 public int areaRectangle(int l, int b){
return l*b;
 }
 public static void main(String args[]){
Area a = new Demo();
System.out.println("Area of square " + a.areaSquare(9));
System.out.println("Area of rectangle " + a.areaRectangle(3,4));
a.display();
 }
}
Output:

Area of square 81

Area of rectangle 12

Normal method in abstract class Area

Final Method in Java
A method that is declared final is called a final method. We cannot override a final method. This means the child class can still call the final method of parent class without any problem, but it cannot override it. This is because the main purpose of making a method final is to stop the modification of the method by the sub-class.

Example:

class DemoParent{  
final void method(){
System.out.println("Parent class final method");
}  
}  
     
class Demo extends DemoParent{  
//error
void method(){
System.out.println("final method modified inside child class");
}  
     
public static void main(String args[]){  
Demo d = new Demo();  
d.method();  
}  
}
The above code will throw an error as we are trying to modify the final method inside the child class(demo) of the parent class(demoParent).

Instead of modifying the method we can use it as shown below:

class DemoParent{  
final void method(){
System.out.println("Parent class final method");
}  
}  
     
class Demo extends DemoParent{
public static void main(String args[]){  
Demo d = new Demo();  
d.method();  
}  
}
Output:

Parent class final method

Equals Method in Java
As the name suggests in java, .equals() is a method used to compare two objects for equality. The .equals() method in java is used to check if the two strings have similar values. It checks them character by character. One should not confuse .equals() method with == operator. The String equals() method compares the two given strings based on the content of the string, whereas the == operator is used for address comparison. If all the contents of both the strings are the same, then .equals() returns true otherwise, it returns false. If all characters are not matched, then it returns false. 

Let us understand this with the help of an example:

public class Demo {
    public static void main(String[] args)
    {
        String s1 = "GreatLearning";
        String s2 = "GreatLearning";
        String s3 = new String("GreatLearning");
        System.out.println(s1 == s2); // true
        System.out.println(s1 == s3); // false
        System.out.println(s1.equals(s2)); // true
        System.out.println(s1.equals(s3)); // true
    }
}
Even though s1 and s3 are created with the same field(content), they are pointing to two different objects in memory. Hence at different addresses. Therefore == operator gives false and .equals() method gives true as both contain similar content greatLearning.

Message Passing in Java
Message Passing in terms of computers is a communication phenomenon between the processes. It is a kind of communication used in object-oriented programming. Message passing in Java is the same as sending an object, i.e., a message from one thread to another thread. It is utilized when threads do not have shared memory and are not able to share monitors or any other shared variables to communicate. In message passing calling program sends a message to a process and relies on that process to run its own functionality or code. Message passing is easy to implement, has faster performance, and we can build massive parallel models by using it. 

There are two types of it: Synchronous and Asynchronous.

Synchronous message passing occurs when the objects run at the same time.
In the case of an Asynchronous message passing, the receiving object can be down or busy when the requesting object sends the message.
Can Polymorphism, Encapsulation and Inheritance work together?
When we combine inheritance, polymorphism and encapsulation to produce a programming environment, this environment supports the development of far more robust and scalable programs that do the program-oriented model. A well designed or model of the hierarchy of classes are the basis for reusing the code in which we have spent our time and effort developing and testing.  Encapsulation allows us to migrate our implementations over time without breaking that code which depends on our classes’ public interfaces. Polymorphism allows us to create a readable, clean, sensible code.

As we know, it is through the applications of encapsulation, polymorphism and inheritance that individual parts are transformed into an object; for example, it may be a car, mobile phone etc. This is true in case of computer programs. Through object-oriented principles, the various parts of complex programs are brought together to form a cohesive, robust, maintainable whole.

Many of the features supplied by java are part of its built-in class libraries which do use encapsulation, polymorphism, and inheritance extensively. 

Let us consider a real-world example. Humans are a form of inheritance at one standpoint, whereas cars are more like programs we write. All drivers rely on inheritance to drive different types of vehicles. People interface with the features on cars of all types as we have many different types of vehicles, and some have differences. The implementation of engines, brakes etc., comes under encapsulation and finally comes to polymorphism. We get a wide area of options on the same vehicle as to the anti-lock braking system, traditional braking system or power braking system. The same vehicle as many forms of the braking system is called polymorphism. This example shows us how encapsulation, inheritance and polymorphism are combined.   

Advantages of OOPs Concept 
OOPs concepts are one of the core development approaches which is widely accepted. Some of the advantages are:

Re-usability
When we say re-usability, it means that “write once, use it multiple times” i.e., reusing some facilities rather than building it again and again, which can be achieved by using class. We can use it n number of times whenever required.

Data redundancy 
It is one of the greatest advantages in oops. This is the condition which is created at the data storage when the same piece of data is held at two different places. If we want to use a similar functionality in multiple classes, we can just write common class definitions for the similar functionalities by inheriting them.

Code maintenance
It is easy to modify or maintain existing code as new objects which can be created with small differences for the existing ones. It also helps users from doing rework many times. It is time saving as we modify the existing codes incorporating new changes to it.

Security
Data hiding and abstraction are used to filter out limited exposure which means we are providing only necessary data to view as we maintain security.

Design benefits 
The designers will have a longer and extensive design phase, which results in better designs. At a point of time when the program has reached critical limits, it will be easier to program all non oops one separately.

Easy troubleshooting
Using encapsulation objects are self-constrained. So, if developers face any problem easily it can be solved. And there will be no possibility of code duplicity. 

Flexibility 
Problem solving
Disadvantages of OOPs Concept 
Effort – Lot of work is put into creating these programs.
Speed – These programs are slower compared to other programs.
Size – OOPs programs are bigger when compared to other programs.
Differences between Object-Oriented Programming, Procedural Oriented Programming, Structured Programming?
Object-oriented programming	Procedure oriented programming
It is object oriented.	It is structured oriented.
It follows a bottom-up approach.	It is divided into small parts called functions.
These are divided into small parts called objects.	It follows a top-down approach.
These have specifiers like public, private, protected.	There are no access specifiers.
Adding new functions or data is easy.	Adding new data and functions is not easy.
It provides data hiding and it is more secure.	This is less secure.
Overloading is possible.	Overloading is not possible.
Examples are c++, java, python etc.	Examples FORTRAN, Cobol etc.
Structured programming 

This divides a program into functions and modules, using this function and modules it makes the program more understandable and readable. It gives importance to functions rather than data and focuses on development on large software applications.
Example c, pascal.
Summary 
OOPs is used to design a program using classes and objects.
OOPs is the core of java.
Objects are instances of classes and also real entities of the world.
Classes are collections of objects; they use keyword class whenever written or named.
Polymorphism means many forms that can be overloaded or overridden.
Abstraction refers to the data hiding, it displays only the information required by the user.
Inheritance is the process of acquiring or inheriting properties of one class to the other.
Encapsulation means wrapping of the data, they use get and set methods.
Oops concepts have re-usability, code maintenance, code redundancy, security etc. 
FAQ
1. What are the OOPS concepts in Java?
OOPs stands for Object-oriented programming. OOPs in Java organizes a program around the various objects and well-defined interfaces. The OOPs Concepts in Java are abstraction, encapsulation, inheritance, and polymorphism. These concepts aim to implement real-world entities in programs.

2. What are the 4 basics of OOP?
The four basics of OOP are abstraction, encapsulation, inheritance, and polymorphism. These are the main ideas behind Java’s Object-Oriented Programming.

3. What are the OOPS concepts in Java with examples?
OOPs concepts in Java is known as object-oriented programming System. The following is a list of the OOPs concepts in Java with examples:
1. Class
2. Object
3. Inheritance
4. Polymorphism
5. Abstraction
6. Encapsulation
7. Association
8. Aggression
9. Composition

4. What explains the concept of Oops?
OOPs help in creating a working method and variable that can be reused without compromising on security. The emphasis of OOPs concepts is on data rather than on functions and is mainly used in different object-oriented programming languages such as Java, C#, C++, Python, Perl, Ruby, etc.

5. What are the main features of OOPs?
The main features of OOPs concepts in Java are Classes, Objects, Encapsulation, Data Abstraction, Polymorphism, Inheritance.

6. Why is OOPs concepts used?
The reason for using OOPs concepts in Java is to implement various real-world entities such as polymorphism, abstraction, inheritance, etc., into programming. Another reason to use this is to ensure security of code by binding together the data and functions.

7. What are the advantages of OOPs?
There are several benefits of implementing OOPs Concepts in Java. A few of the major advantages are as follows: Re-usability, Code maintenance, Data Redundancy, Security, Easy troubleshooting, Problem-Solving, Flexibility and Design Benefits. Java OOPs Concepts are one of the core development approaches that is widely accepted.

8. What is polymorphism in OOPs?
In OOPs, Polymorphism is the process that allows us to perform a single action in multiple ways. This occurs when there are several classes related to each other through inheritance. In polymorphism, there are two types. Namely, compile-time polymorphism and runtime polymorphism. It helps us in reducing complexity.

This brings us to the end of the blog on OOPS concepts in Java. If you found this helpful and wish to learn more such concepts, you can check out the free courses available on Great Learning Academy.
