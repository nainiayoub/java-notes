## Introduction
This repository contains my personnal notes and questions, that I have managed to answer, related to the general-purpose programming language __JAVA__. These notes will cover ___JAVA Basics___, ___OOP___, ___Inheritance___ and much more. This repository is intended to be used as a reminder of JAVA concepts.
## Table of contents
* [Introduction](#Introduction)
* __Java Basics__
    * [What is the difference between JDK and JRE?](#what-is-the-difference-between-jdk-and-jre)
    * [What is Java Virtual Machine (JVM)?](#what-is-java-virtual-machine-jvm)
    * [What are the different types of memory areas allocated by JVM?](#what-are-the-different-types-of-memory-areas-allocated-by-jvm)
    * [What is JIT compiler?](#what-is-jit-compiler)
    
## What is the difference between JDK and JRE?
<img src="https://lh3.googleusercontent.com/proxy/3mROJt4It2-QP2JQb5aW4fCgXa1HzvKioZTC734RpDnSKVHQ2WUvWyF0qX8jabPJOe28QxxeYVmSbUTu04C9ATbIjOmDkX5CeaNVm3b7ajCiKQk4msEnWY2UU3HykPkd" alt="Description of Java Conceptual Diagram"><br/>
#### JRE (Java Runtime Environment)
* The `JRE` is used to run your Java program. It includes the `JVM`, a set of libraries that come with Java as well as `Java Launcher`.
* The `JRE` doesn't include any development tools.
#### JDK (Java Development Kit)
* The `JDK` is the development kit that you need to create Java programs. 
* The `JDK` is basically the tools that will take your Java source code and convert it into a format that the `JRE` and the `JVM` can execute.
* The `JDK` comes bundled with a Java Runtime Edition as shown in the Image above.

Back to Top :point_up: [Table of contents](#table-of-contents)

## What is Java Virtual Machine (JVM)?
<img src="https://math.hws.edu/javanotes/c1/overview-fig3.png" alt="Java Virtual Machine"><br/>
* The `JVM` (Java Virtual Machine) is a run-time engine that converts `Java bytecode` _(generated by `the Compiler`)_, thanks to The `Execution engine` into machine code.
* The `JVM` is a part of [Java Runtime Environment (JRE)](#jre-java-runtime-environment), which means that it enables a computer to run Java programs as well as programs written in other languages that are also compiled to Java bytecode.
* The `JVM` is the one that actually calls the main method present in a java code.
* The `JVM` resides on the RAM.

Back to Top :point_up: [Table of contents](#table-of-contents)

## What are the different types of memory areas allocated by JVM?
All objects created in Java are stored in `JVM (Java virtual machine)`. JVM memory is basically divided into the following parts:
1. Method Area.
2. Heap Memory.
3. Stack Memory.
4. Program Counter register.
5. Native method Stacks.

## What is JIT compiler?
<img src="https://www.edureka.co/blog/wp-content/uploads/2019/06/JIT-Compiler-JIT-in-Java-Edureka-2.png" alt="Just-In-Time compiler" width="50%"><br/>
* The `Just-In-Time (JIT) compiler` is a an essential part of the JRE, that improves the performance of Java applications by compiling platform-neutral Java bytecode into native machine code at run time.
* Without `the JIT`, the JVM has to interpret the bytecodes itself - a process that requires extra CPU and memory.
