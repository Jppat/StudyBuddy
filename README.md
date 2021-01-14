# StudyBuddy
Repository for CMSC123 Final Project (StudyBuddy)
by: Jppat

## Project Description
I made the program Study Buddy to help me become organized with my syllabus. Although copies are distributed by instructors during the start of the term, I tend to lose mine. Also, sometimes I get overwhelmed with the amount of papers related to school that I have to keep track with. I acknowledge that there are apps with similar focus on academic productivity. However, Study Buddy is just my personal program to help me back on track with my academic responsibilities using a simple interface.

## TDD
For the development of the project I used JUnit as the tool for the Test Driven Development Framework.

## Design Patterns

Creational Design Pattern -
* Prototype Pattern : 
The prototype pattern was employed in the creation of a curriculum object. The class curriculum houses all the attributes that a curriculum has.
To make a new curriculum object, the prototype for a curriculum is clone instead of instantiating a new Curriculum object.

Structural Design Pattern -
* Composite Pattern : 
The goal of the composite pattern is to be able to treat individual and grouped subjects just as you would with an indivual object. Since, by nature the majority of the elements of the program is composed of individual objects which are aggregated into lists, I made the decision to incorporate the principles of the Composite Design Pattern in organizing my program's elements.

For instance, both Classes Course and CourseList implement interfaces which extend the DisplayInterface. To display items of a list object, the list class delegates the work to its individual objects to call the display method. Both the Object Class and the ObjectList class use the same display method.

Behavioral Design Pattern -
* Template Method :
In the template method, an algorithm's skeleton structure is defined in an abstract class or in an interface, letting subclasses inherit the same structure but with the option of overriding some depending on the specifications of that subclass.

The template method is used with the structure of the program's Individual Object Classes : Curriculum, Course and Topic. All three extend the abstract class 'Item' which defines methods and attributes common to the three classes. These classes differ only in the implementation of their associated ObjectList classes.

## Best Practices Used
* Naming conventions such as starting out with UpperCase characters for Class Names, LowerCase characters for methods with the next word --- for both Class Names and Method Names --- in Uppercase (CamelCase) and package names written in lowercase.
* Consistency with the use of tab when indenting lines/blocks of code.
* Placing declarations of commonly used variables at the beginning of a block.
``` java
static String action;
static String name;
static String mode;
static int index;

//methods
```
* Adding one line of space after every method.
