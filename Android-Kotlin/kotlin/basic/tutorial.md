# 1. Introduction
  - kotlin (was released in 2016 by JetBrains.)
    1. modern, trending programming language.
    2. easy to learn.
    3. 100% compatible with java.
    
  - Kotlin is used for:
    - Moblie Applications (specially Android Apps)
    - Web development
    - Sever side applications
    - Data Science
    - etc...

  - Why use kotlin?
    - Kotlin is full compatible with Java.
    - Kotlin works on different platforms (windows, mac, linux, Raspberry Pi, etc...)
    - Kotlin is concise and afe
    - easy to learn.
    - Free to use.
    - Big community / Suport.

  - Kotlin Install
    1. Install Java.
      - install zulu sdk
        - [zulu sdk](https://www.azul.com/)
        - [how to install](https://blog.naver.com/picassozin/222354057305)
    2. Install IntelliJ.(IDE)

# 2. Syntax
```kotlin
fun main() {
  println("Hello World")
}
```
- ```fun``` : used to declare a function.
  - A function is a block of code designed to perform a particular task.
  - (in the example...) It declares the ```main()``` functions.

- ```main()``` : **execute** code.
  - Andy code inside the ```main()``` function's curly brackets ```{}``` will be **executed.**
  - executed : 실행

> Good To Know : In kotlin, code statements do not have to end with a semicolon (;)

- Main Parameters
  - Before Kotlin version 1.3, it was required to use the ```main()``` function with parameters, like : ```fun main(arg : Array<String>).```
  - The example above hhad to be written like this to work:
    ```kotlin
    fun main(args : Array<String>) {
        println("Hello World")
    }
    ```
    
- ```println()```, ```print()```
  - ```print()``` function is similar to ```println()```. The only difference is that it does not insert a new line at the end of the output.

# 3. Variables
- To create a variable, use ```var``` or ```val```, and assign a value to it with the equal sign (```=```).
  ```kotlin
  var variableName = value
  val variableName = value
  ```
  
  - example
  ```kotlin
  var name = "John"
  val birthyear = 1975
  
  println(name)
  println(birthyear)
  ```
  
  - The difference between ```var``` and ```val```is that variables declared with the ```var``` keyword **can be changed/modified**, while ```val``` variables **cannot**.
  - Therefore, ```var``` variables can be changed/modified, but ```val``` variables can not be changed/modified.

- Variable Type
  - Unlike many other programming languages, variable in Kotlin do not need to be declared with a specified type.
  - To create a variable in Kotlin that should store text and another that should store a number, look at the following example:
  
  ```Kotlin
  // example.kt
  var name = "John"    // String (text)
  val birthyear = 1975 // Int (number)
  
  println(name)
  println(birthyear)
  ```
  
  - Kotlin is smart enough to understand that "John" is a ```String```(text), and that **1975** is an ```Int``` (number) variable.
  - However, it is possible to specify the type if you instst:
  ```kotlin
  var name: String = "John"  // String
  val birthyear: Int = 1975  // Int
  
  println(name)
  println(birthyear)
  ```
  
  - You can also declare a variable without assign the value, and assign the value later.
  - However, this is only possible when you specify the type:
  - This works fine:
  ```kotlin
  var name: String
  name = "John"
  println(name)
  ```
  
  - This will generate an error:
  ```kotlin
  var name
  name = "John"
  println(name)
  ```
  
- Note on ```val```
  - ```val``` value cannot be changed/reassigned.
  ```kotlin
  val name = "John"
  name = "Robert"  // Error! (use var!)
  println(name)
  ```
  
  - So... The ```val``` keyword is useful when you want a variable to always store the same value, like PI, e, ...

- ```println()``` method can use ```+``` character.
  - ```+``` character use to combine both text and a variagble.
  ```kotlin
  val name = "John"
  println("Hello " + name)
  
  val x = 5
  val y = 6
  println(x + y) // 11
  ```
  
- Variable Names
  - The general rule for Kotlin variables are:
    - Names can contain letters, digits, underscores, and dollar signs.
    - Names should start with a letter.
    - Names can also begin with $ and _.
    - Names are case sensitive. ("myVar" and "myvar" are different variables)
    - Names should start with a lower case letter and it cannot contain whitespace.
    - Reserved Words (ex : var, String) cannot be used as names.
  - (Recommended Notation : camelCase Notation)