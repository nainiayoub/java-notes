## Introduction
This repository contains my personnal notes and questions, that I have managed to answer, related to the general-purpose programming language __JAVA__. These notes will cover ___JAVA Basics___, ___OOP___, ___Inheritance___ and much more. This repository is intended to be used as a reminder of JAVA concepts.
## Table of contents
* [Introduction](#Introduction)
* __Java Basics__
    * [What is the difference between JDK and JRE?](#what-is-the-difference-between-jdk-and-jre)
    * [What is Java Virtual Machine (JVM)?](#what-is-java-virtual-machine-jvm)
    * [What are the different types of memory areas allocated by JVM?](#what-are-the-different-types-of-memory-areas-allocated-by-jvm)
    * [What is JIT compiler?](#what-is-jit-compiler)
    * [How Java platform is different from other platforms?](#how-java-platform-is-different-from-other-platforms)
    * [Why Java is 'write once and run anywhere' language?](#why-java-is-write-once-and-run-anywhere-language)
    * [How does ClassLoader work in Java?](#how-does-classloader-work-in-java)
    * [Is ‘main’, used for main method, a keyword in Java?](#is-main-used-for-main-method-a-keyword-in-java)
    * [Can we write main method as static public void instead of public static
void?](#can-we-write-main-method-as-static-public-void-instead-of-public-static-void)
    * [In Java, if we do not specify any value for local variables, then what
will be the default value of the local variables?](#in-java-if-we-do-not-specify-any-value-for-local-variables-then-what-will-be-the-default-value-of-the-local-variables)
    * [What is the difference between byte and char data types in Java?](#what-is-the-difference-between-byte-and-char-data-types-in-java)
    * [What is the difference between static method and instance method in Java?](#what-is-the-difference-between-static-method-and-instance-method-in-java)
    
* __Object-Oriented Programming System (OOPs)__
    * [What are the main principles of Object Oriented Programming?](#what-are-the-main-principles-of-object-oriented-programming)
    * [What is the difference between Object Oriented Programming language and Object Based Programming language?](#what-is-the-difference-between-object-oriented-programming-language-and-object-based-programming-language)
    * [In Java what is the default value of an object reference defined as an instance variable in an Object?](#in-java-what-is-the-default-value-of-an-object-reference-defined-as-an-instance-variable-in-an-object)
    * [Why do we need default constructor in Java classes?](#why-do-we-need-default-constructor-in-java-classes)
    * [Can we inherit a Constructor?](#can-we-inherit-a-constructor)
    * [Why constructors cannot be final, static, or abstract in Java?](#why-constructors-cannot-be-final-static-or-abstract-in-java)
 
* __Inheritance__
    * [Explain the concept of Inheritance?](#explain-the-concept-of-inheritance)
    * [Which class in Java is superclass of every other class?](#which-class-in-java-is-superclass-of-every-other-class)
    * [Why Java does not support multiple inheritance?](#why-java-does-not-support-multiple-inheritance)
    * [In OOPS, what is meant by composition?](#in-oops-what-is-meant-by-composition)
    * [How aggregation and composition are different concepts?](#how-aggregation-and-composition-are-different-concepts)
    * [If there are no pointers in Java, then why do we get NullPointerException?](#if-there-are-no-pointers-in-java-then-why-do-we-get-nullpointerexception)
    * [What is the purpose of ‘super’ keyword in Java?](#what-is-the-purpose-of-super-keyword-in-java)
    * [What is the meaning of object cloning in Java?](#what-is-the-meaning-of-object-cloning-in-java)
    
* __Static__
    * [In Java, why do we use static variable?](#in-java-why-do-we-use-static-variable)
    * [Why it is not a good practice to create static variables in Java?](#why-it-is-not-a-good-practice-to-create-static-variables-in-java)
    * [What is the purpose of static method in Java?](#what-is-the-purpose-of-static-method-in-java)
    * [Why do we mark main method as static in Java?](#why-do-we-mark-main-method-as-static-in-java)
    * [In what scenario do we use a static block?](#in-what-scenario-do-we-use-a-static-block)
    * [Is it possible to execute a program without defining a main() method?](#is-it-possible-to-execute-a-program-without-defining-a-main-method)
    * [What happens when static modifier is not mentioned in the signature of main method?](#what-happens-when-static-modifier-is-not-mentioned-in-the-signature-of-main-method)
    * [What is the difference between static method and instance method in Java?](#what-is-the-difference-between-static-method-and-instance-method-in-java)

* __Method Overloading and Overriding__
    * [What is the other name of Method Overloading?](#what-is-the-other-name-of-method-overloading) 
    * [How will you implement method overloading in Java?](#how-will-you-implement-method-overloading-in-java)
    * [Why it is not possible to do method overloading by changing return type of method in java?](#why-it-is-not-possible-to-do-method-overloading-by-changing-return-type-of-method-in-java)
    * [Is it allowed to overload main() method in Java?](#is-it-allowed-to-overload-main-method-in-java)
    * [How do we implement method overriding in Java?](#how-do-we-implement-method-overriding-in-java)
    * [Why Java does not allow overriding a static method?](#why-java-does-not-allow-overriding-a-static-method)
    * [Is it allowed to override an overloaded method?](#is-it-allowed-to-override-an-overloaded-method)
    * [What is the difference between method overloading and method overriding in Java?](#what-is-the-difference-between-method-overloading-and-method-overriding-in-java)
    * [What is meant by covariant return type in Java?](#what-is-meant-by-covariant-return-type-in-java)
    
* __Polymorphism__ 
    * [What is Runtime Polymorphism?](#what-is-runtime-polymorphism)
    * [Is it possible to achieve Runtime Polymorphism by data members in Java?](#is-it-possible-to-achieve-runtime-polymorphism-by-data-members-in-java)
    * [Explain the difference between static and dynamic binding?](#explain-the-difference-between-static-and-dynamic-binding)
    
* __Abstraction__ 
    * [What is Abstraction in Object Oriented programming?](#what-is-abstraction-in-object-oriented-programming)
    * [How is Abstraction different from Encapsulation?](#how-is-Abstraction-different-from-encapsulation)

# Java Basics
## What is the difference between JDK and JRE?
<img src="https://devops.com.vn/wp-content/uploads/2018/07/jdk_jre_jvm.png" alt="Description of Java Conceptual Diagram"><br/>
#### JRE (Java Runtime Environment)
* The `JRE` is used to run your Java program. It includes the `JVM`, a set of libraries that come with Java as well as `Java Launcher`.
* The `JRE` doesn't include any development tools.
#### JDK (Java Development Kit)
* The `JDK` is the development kit that you need to create Java programs. 
* The `JDK` is basically the tools that will take your Java source code and convert it into a format that the `JRE` and the `JVM` can execute.
* The `JDK` comes bundled with a Java Runtime Edition as shown in the Image above.

__Back to Top__ :point_up: [Table of contents](#table-of-contents)

## What is Java Virtual Machine (JVM)?
<img src="https://math.hws.edu/javanotes/c1/overview-fig3.png" alt="Java Virtual Machine"><br/>
* The `JVM` (Java Virtual Machine) is a run-time engine that converts `Java bytecode` _(generated by `the Compiler`)_, thanks to The `Execution engine` into machine code.
* The `JVM` is a part of [Java Runtime Environment (JRE)](#jre-java-runtime-environment), which means that it enables a computer to run Java programs as well as programs written in other languages that are also compiled to Java bytecode.
* The `JVM` is the one that actually calls the main method present in a java code.
* The `JVM` resides on the RAM.

__Back to Top__ :point_up: [Table of contents](#table-of-contents)

## What are the different types of memory areas allocated by JVM?
All objects created in Java are stored in `JVM (Java virtual machine)`. JVM memory is basically divided into the following parts:
1. Method Area.
2. Heap Memory.
3. Stack Memory.
4. Program Counter register.
5. Native method Stacks.

## What is JIT compiler?
<img src="https://www.edureka.co/blog/wp-content/uploads/2019/06/JIT-Compiler-JIT-in-Java-Edureka-2.png" alt="Just-In-Time compiler" width="60%"><br/>
* The `Just-In-Time (JIT) compiler` is a an essential part of the JRE, that improves the performance of Java applications by compiling platform-neutral Java bytecode into native machine code at run time.
* Without `the JIT`, the JVM has to interpret the bytecodes itself - a process that requires extra CPU and memory.

__Back to Top__ :point_up: [Table of contents](#table-of-contents)

## How Java platform is different from other platforms?
<img src="https://docs.oracle.com/javase/tutorial/figures/getStarted/getStarted-jvm.gif" alt="Java platform"><br/>
* Most platforms can be described as a combination of the operating system and underlying hardware. The Java platform differs from most other platforms in that it's a software-only platform that runs on top of other hardware-based platforms.
* The Java platform has two components:
   * [The Java Virtual Machine](#what-is-java-virtual-machine-jvm).
   * The Java Application Programming Interface (API).
   * Java is platform independent (WORA).
   
## Why Java is 'write once and run anywhere' language?
* Java applications are called `WORA (Write Once Run Anywhere)`. This means Java can be developed on any device, compiled into a standard bytecode and be expected to run on any device equipped with a JVM.
*  __Java is portable__, means that you can run Java bytecode on any hardware that has a compliant [JVM (Java Virtual Machine)](#what-is-java-virtual-machine-jvm).

__Back to Top__ :point_up: [Table of contents](#table-of-contents)

## How does ClassLoader work in Java?
### What is ClassLoader in Java?
ClassLoader in Java is a class that is used to load `class files in Java`. Java code is compiled into a class file by `javac compiler` and JVM executes Java program, by executing byte codes written in the class file. __ClassLoader is responsible for loading class files from file systems, networks, or any other source__. 
### How does it work?
Java class loaders are used to load classes at runtime. ClassLoader in Java works on three principles: `delegation, visibility, and uniqueness`.
* `Delegation principle` forward request of class loading to parent class loader and only loads the class if the parent is not able to find or load the class.
* `Visibility principle` allows child class loader to see all the classes loaded by parent ClassLoader, but parent class loader can not see classes loaded by a child.
* `Uniqueness principle` allows one to load a class exactly once, which is basically achieved by delegation and ensures that child ClassLoader doesn't reload the class already loaded by a parent.

Correct understanding of class loader is a must to resolve issues like `NoClassDefFoundError` in Java and `java.lang.ClassNotFoundException`, which are related to class loading.

__Back to Top__ :point_up: [Table of contents](#table-of-contents)

## Is ‘main’, used for main method, a keyword in Java?
* In Java, __`main`__ is the name of Java main method. It is the identifier that the JVM looks for as the starting point of the java program. __It’s not a keyword__. 

## Can we write main method as static public void instead of public static void?
* If you write `static public void main` instead of `public static void main`, then it will make no difference. Program compiles properly and runs. But if you change the sequence of main, then it will you give a compiler error.
* In Java, __we can declare access modifiers in any order__, the method name comes last, the return type comes second to last and then after it's our choice. But __it's recommended to put access modifier (public, private and protected) at the forefront as per Java coding standards__.

## In Java, if we do not specify any value for local variables, then what will be the default value of the local variables?
* There is no default value for local variables, so local variables should be declared and an initial value should be assigned before the first use.
* Using a local variable without initializing would give an error at the time of compilation.

__Back to Top__ :point_up: [Table of contents](#table-of-contents)


## What is the difference between byte and char data types in Java?
1. The first and foremost difference between byte and char are that __byte is a signed data type while char is an unsigned data type__.
2. From above fact, we can deduce another difference between byte and char. __Byte can represent negative values but char values are always positive__.
3. Another difference between char and byte is that char is a larger data type than a byte. __The range of byte is between -128 to 127 but the range of char is from 0 to 65535__, because byte is a signed 8-bit data type and char is an unsigned 16-bit data type hence, its maximum value is 2 ^ 16 - 1 which is 65535.

# Object-Oriented Programming System (OOPs)
## What are the main principles of Object Oriented Programming?
* There are 4 major principles that make a language Object Oriented. These are __Encapsulation__, __Data Abstraction__, __Polymorphism__ and __Inheritance__. 

## What is the difference between Object-Oriented Programming language and Object Based Programming language?
In computer science, the term object-based has two different senses:
* A limited version of object-oriented programming, where one or more of the following restrictions applies: 
   * There is no implicit inheritance.
   * There is no polymorphism. 
   * Only a very reduced subset of the available values are objects (typically the GUI components).
* Prototype-based systems (that is, those based on "prototype" objects that are not instances of any class).

The core difference between the two is that an object-oriented programming language has the features that an object-oriented paradigm must have in order to be considered an object-oriented programming language. While object based programming languages are __Prototype-based__ where one or more of OOP principles are lacking.

## In Java what is the default value of an object reference defined as an instance variable in an Object?
* The object references are all initialized to null in Java. However in order to do anything useful with these references, you must set them to a valid object, else you will get `NullPointerExceptions` everywhere you try to use such default initialized references.

__Back to Top__ :point_up: [Table of contents](#table-of-contents)

## Why do we need default constructor in Java classes?
* The compiler automatically provides a public no-argument constructor for any class without constructors. This is called the __default constructor__.
* This default constructor initializes the variables of the class with their respective default values (null for objects, 0.0 for float and double, false for boolean, 0 for byte, short, int and, long).

## Can we inherit a Constructor?
* Constructors are not inherited. They are called implicitly or explicitly by the child constructor.
* A subclass inherits all the members (fields, methods, and nested classes) from its superclass. Constructors are not members, so they are not inherited by subclasses, but the constructor of the superclass can be invoked from the subclass.

## Why constructors cannot be final, static, or abstract in Java?
* Constructors can't be final because when we say a method is final that means it can't be overriden. Constructors by Java rules can't be overriden anyways so there is no point in making constructors as final.
* Static methods belong to the class. Whereas a Constructor belongs to the object and called when we use the new operator to create an instance. Since a constructor is not class property, it makes sense that it’s not allowed to be static. (Constructors are implicitly final and static, you don’t need to declare it again)
* Constructors can’t be abstract because when you set a method as ‘abstract’, it means method doesn't have any body and you want to implement it at another time in a child class, but the constructor is called implicitly when the new keyword is used so it can’t lack a body.

# Inheritance
## Explain the concept of Inheritance?
* Inheritance is a proces in which one class acquires the properties (fields and methods) of an other.
* With inheritance, we can reuse the fields and methods of the existing class. Hence, __inheritance facilitates Reusability__ and is an important concept of OOPs.
* The class which inherits the properties of other is known as subclass (derived class, child class) and the class whose properties are inherited is known as superclass (base class, parent class).

## Which class in Java is superclass of every other class?
* The __Object class__, which is stored in the `java.lang package`, is the ultimate superclass of all Java classes. Because of this, all Java classes inherit methods from `Object`. Half of these methods are final and cannot be overridden.

## Why Java does not support multiple inheritance?
* Multiple Inheritance is a feature of object oriented concept, where a class can inherit properties of more than one parent class. The problem occurs when there exist methods with same signature in both the super classes and subclass. __On calling the method, the compiler cannot determine which class method to be called and even on calling which class method gets the priority__.
* Multiple inheritance is not supported by Java using classes , handling the complexity that causes due to multiple inheritance is very complex. It creates problem during various operations like casting, constructor chaining etc and there are very few scenarios on which we actually need multiple inheritance, so better to omit it for keeping the things simple and straightforward.

__Back to Top__ :point_up: [Table of contents](#table-of-contents)

## In OOPS, what is meant by composition?
* Composition is one of the fundamental concepts in object-oriented programming. It describes a class that references one or more objects of other classes in instance variables. This allows you to model a has-a association between objects.

## How aggregation and composition are different concepts?
Both __Aggregation__ and __Composition__ are specific cases of __Association__. In both aggregation and composition object of one class owns object of another class. But there is a subtle difference : 
* __Aggregation__ implies a relationship where the child can exist independently of the parent. Example: Class (parent) and Student (child). Delete the Class and the Student still exist. 
* __Composition__ implies a relationship where the child cannot exist independent of the parent. Example: House (parent) and Room (child). Rooms don't exist separate to a House.

## If there are no pointers in Java, then why do we get NullPointerException?
__Java doesn’t support pointer explicitly, but it uses pointer implicitly :__ 
* Java use pointers for manipulations of references but these pointers are not available for outside use. Any operations implicitly done by the language are actually NOT visible.
* NullPointerException is a RuntimeException. In Java, a special null value can be assigned to an object reference. __NullPointerException is thrown when program attempts to use an object reference that has the null value__.

## What is the purpose of ‘super’ keyword in java?
* The super keyword refers to superclass (parent) objects. 
* The super keyword is used to call superclass methods, and to access the superclass constructor. 
* The most common use of the super keyword is to eliminate the confusion between superclasses and subclasses that have methods with the same name.

## What is the meaning of object cloning in Java?
* Object cloning refers to creation of exact copy of an object. It creates a new instance of the class of current object and initializes all its fields with exactly the contents of the corresponding fields of this object.
* The class whose object’s copy is to be made must have a public clone method in it or in one of its parent class.

__Back to Top__ :point_up: [Table of contents](#table-of-contents)

# Static
## In Java, why do we use static variable?
* We use static variables when only one copy of the variable is required. Variables declared static are commonly shared across all instances of a class.
* Static variables reduce the amount of memory used by a program. Static variables are shared among all instances of a class. 

## Why it is not a good practice to create static variables in Java?
Much as it’s often said that “Inheritance breaks encapsulation” statics do this in a far more severe way, by not just exposing internal implementation but also by exposing internal state.
* The problem is when a variable can be altered by any instance of a class then the fundamental principle behind encapsulation/information hiding is lost entirely: __An object is no longer in complete control of its state__.
* Any instance of the object can alter the static variable which causes ambiguity as individual instances of the object no longer have control over their own state. 
* State changes can arbitrarily happen without knowledge of an object which relies on that state which is problematic because the object may not work correctly when this happens. 

## What is the purpose of static method in Java?
* We use static method when we want to provide class level access to a method, where the method should be callable without an instance of the class. Static methods don't need to be invoked on the object and that is when you use it.

## Why do we mark main method as static in Java?
* Java main() method is always static, so that compiler can call it without the creation of an object or before the creation of an object of the class.
* If the main() is allowed to be non-static, then while calling the main() method JVM has to instantiate its class.
* The main() method in Java must be declared public, static and void. If any of these are missing, the Java program will compile but a runtime error will be thrown.

__Back to Top__ :point_up: [Table of contents](#table-of-contents)

## In what scenario do we use a static block?
* We use a static block when a class that has static members requires initialization. 
* The code inside static block is executed only once, the first time the class is loaded into memory. 
* Static blocks are executed before constructors.

## Is it possible to execute a program without defining a main() method?
* Yes, we can execute a JAVA program without a main method by using a __static block__.
* In the example below, we can execute a JAVA program without a main method (works until Java 1.6 version). 
```
class StaticInitializationBlock{
   static{
      System.out.println("class without a main method");
      System.exit(0);
   }
}
```
* Java 7 and newer versions don’t allow the execution of a JAVA program because JVM checks the presence of the main method before initializing the class.

## What happens when static modifier is not mentioned in the signature of main method?
* Without having declared main method static , our program will successfully compile but won't execute and report error at run time. 
* Declaring main method static is necessary since main is called by the Java interpreter before any objects are made. 
* Since keyword static allows main to be called without creating an object of the class in which the main method is defined, our main method needs to be declared static.

## What is the difference between static method and instance method in Java?
* __Instance methods__ are methods which require an object of its class to be created before it can be called. 
   * To invoke a instance method, we have to create an Object of the class in within which it defined.
   * Instance method(s) belong to the Object of the class not to the class. they can be called after creating the Object of the class.
   * Every individual Object created from the class has its own copy of the instance method(s) of that class.
   * They can be overridden since they are resolved using dynamic binding at run time.
   
* __Static methods__ are the methods in Java that can be called without creating an object of class. 
   * They are referenced by the class name itself or reference to the Object of that class.
   * Static method(s) are associated to the class in which they reside. they can be called even without creating an instance of the class.
   * They are designed with aim to be shared among all Objects created from the same class.
   * They can not be overridden. But can be overloaded since they are resolved using static binding by compiler at compile time.

__Back to Top__ :point_up: [Table of contents](#table-of-contents)

# Method Overloading and Overriding
## What is the other name of Method Overloading?
* Method Overloading is also known as __Compile time Polymorphism__ or static polymorphism.

## How will you implement method overloading in Java?
* We can implement method overloading in two different ways:
   * Implementing two or more methods that have the same name but __take different numbers of arguments__.
   * Implementing two or more methods that have the same name but __take arguments of different types__.

## Why it is not possible to do method overloading by changing return type of method in java?
* Java can distinguish the methods with different method signatures. The methods can have same name but with different parameters list (number of the parameters, order of the parameters, and data types of the parameters) within the same class.
* The compiler does not consider the return type while differentiating the overloaded method. But you cannot declare two methods with the same signature and different return type. It will throw a compile time error.
* If both methods have same parameter types, but different return type, then it is not possible to do method overloading.

## Is it allowed to overload main() method in Java?
* Yes, just like anyother method in java, the main method can be overloaded in a similar manner but JVM only calls the original main method, it will never call our overloaded main method.
* In order for the overloaded main method to be executed , we need to call it from the actual main method.

__Back to Top__ :point_up: [Table of contents](#table-of-contents)

## How do we implement method overriding in Java?
* Overriding is a feature that allows a child class to provide a specific implementation of a method that is already provided by one of its parent classes.
* Method Overriding is implemented when a method in a subclass has the same name, same parameters or signature, and same return type(or sub-type) as a method in its super-class, only then the method in the subclass is said to override the method in the super-class.

## Why Java does not allow overriding a static method?
* Java doesn't allow overriding a static method even though we can declare static methods with same signature in subclass, but it is not considered overriding as there won’t be any run-time polymorphism.
* If a derived class defines a static method with same signature as a static method in base class, the method in the derived class hides the method in the base class.

## Is it allowed to override an overloaded method?
* A method can be an override for an overloaded method in a superclass. And you can overload a method that you are simultaneously overriding using another method. 
* You cannot have one method that is both a new overload and an override. 
* For a method to be an override, another method with the same signature must already exist in the superclass, and that means that this method cannot be a new override.

## What is the difference between method overloading and method overriding in Java?
* The most basic difference is that overloading is being done in the same class while for overriding base and child classes are required. 
* __Overriding__ is all about giving a specific implementation to the inherited method of parent class while method __Overloading__ is about allowing a class to have more than one method having the same name, if their argument lists are different.

## What is meant by covariant return type in Java?
* Covariant return type refers to return type of an overriding method. It allows to narrow down return type of an overridden method without any need to cast the type or check the return type. 
* Covariant return type in java means that overriding method can return SubClass.
* Covariant return type works only for non-primitive return types.

__Back to Top__ :point_up: [Table of contents](#table-of-contents)

# Polymorphism
## What is Runtime Polymorphism?
* __Run-time Polymorphism__, also known as __Dynamic Method Dyspatch__, is a process in which a call to an overridden method is resolved at runtime rather than compile-time. 
* Method invocation is determined by JVM not compiler

## Is it possible to achieve Runtime Polymorphism by data members in Java?
* A method is overridden, not the data members, so runtime polymorphism can't be achieved by data members. 

## Explain the difference between static and dynamic binding?
If linking between method call and method implementation is resolved at compile time then we call it __static binding__ or if it is resolved at run time then it __dynamic binding__.
* __Static Binding__ happens at compile time while __Dynamic Binding__ happens at runtime.
* __Static binding__ uses type of the class and fields but __Dynamic binding__ uses object to resolve binding. 
* Overloading is an example of static binding while Method overriding is the example of Dynamic binding.

__Back to Top__ :point_up: [Table of contents](#table-of-contents)

# Abstraction
## What is Abstraction in Object Oriented programming?
* __Abstraction__ is one of the key concepts of object-oriented programming languages. 
* Its main goal is to __handle complexity by hiding unnecessary details from the user__. That enables the user to implement more complex logic on top of the provided abstraction without understanding or even thinking about all the hidden complexity.
* Objects in an OOP languages provide an abstraction that hides the internal implementation details, you just need to know which methods of the object are available to call and which input parameters are needed to trigger a specific operation. But you don’t need to understand how this method is implemented and which kinds of actions it has to perform to create the expected result.

## How is Abstraction different from Encapsulation?
<img src="https://www.topjavatutorial.com/wp-content/uploads/2017/02/Abstraction-and-Encapsulation-new.jpg"><br/>
* __Abstraction__ hides details at the design level, while __Encapsulation__ hides details at the implementation level.
* __Abstraction__ lets you focus on what the object does instead of how it does it, while __Encapsulation__ means hiding the internal details of how an object works.
* __Abstraction__ is about hiding unwanted details while giving out the most essential details, while __Encapsulation__ means hiding the code and data into a single unit e.g. class or method to protect the inner working of an object from the outside world.

