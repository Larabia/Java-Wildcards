# Java-Wildcards 🚀
You can use this project as a cheatsheet or a fast course on Java Wildcards!

Before we start ✋
In this ReadMe you'll find information about Wildcards in Java.
Also, this project includes java files with the actual implementation of Wildcards.

We will be reviewing the following topics:
- Upper Bounded Wildcards.
- Lower Bounded Wildcards.
- Unbounded Wildcard.

You can use this ReadMe as a cheatsheet and clone this project to run it in your IDE for further knowledge about how Wildcards work in Java.

🛠️ This project was created with Java8 and Eclipse(IDE).

So you'll need a basic knowledge  of Java, an IDE and Java 8 installed and you are ready to go!

To download and install Eclipse on Windows 10

To download and install Java8

## Wildcards in Java 🃏

The **question mark (?)** known as the **wildcard** in generic programming **represents an unknown type**.  
Unlike arrays, different instantiations of a generic type are not compatible with each other, not even explicitly. This incompatibility may be softened by the wildcard if ? is used as an actual type parameter.

## 1. Upper Bounded Wildcards ☝️:

To declare an **upper-bounded wildcard**, use the wildcard character `?`, followed by the `extends` keyword, followed by its **upper bound**. 

```java
public static void add(List<? extends Number> list)

```
These wildcards can be used when you want to **relax the restrictions on a variable**. For example, say you want to write a method that works on List < Integer >, List < Double >, and List < Number >, you can do this using an upper bounded wildcard. 

## 2. Lower Bounded Wildcards 👇: 

It is expressed using the wildcard character `?`, followed by the `super` keyword, followed by its **lower bound**: <? super A>. 

```java 
 Syntax: Collectiontype <? super A>
 ```
 
## 3. Unbounded Wildcard 🙃: 
 
This wildcard type is specified using the wildcard character `?`, for example, List. This is called a **list of unknown types**.  
These are useful in the following cases:

- When writing a method that can be employed using functionality provided in Object class.
= When the code is using methods in the generic class that doesn’t depend on the type parameter.


> Use **extend wildcard** when you want to **get values** out of a structure.
> Use **super wildcard** when you **put values** in a structure. 
> **Don’t use wildcard** when you **get and put values** in a structure. You can specify an upper bound for a wildcard, or you can specify a lower bound, but **you cannot specify both**.
