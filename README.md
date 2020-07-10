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

## Is ‘main’, used for main method, a keyword in Java?
* In Java, __`main`__ is the name of Java main method. It is the identifier that the JVM looks for as the starting point of the java program. __It’s not a keyword__. 

## Can we write main method as static public void instead of public static void?
* If you write `static public void main` instead of `public static void main`, then it will make no difference. Program compiles properly and runs. But if you change the sequence of main, then it will you give a compiler error.
* In Java, __we can declare access modifiers in any order__, the method name comes last, the return type comes second to last and then after it's our choice. But __it's recommended to put access modifier (public, private and protected) at the forefront as per Java coding standards__.

