---
layout: post
title:  Kotlin Learning
date:   2023-05-06 14:02:25 +0900
categories: development

---

## Kotlin

---

**What is Kotlin?**

Kotlin is a statically typed programming language developed by JetBrains.

It was created near 2011, and its popularity had increased steadily.

![image](https://i0.wp.com/theengineerscafe.com/wp-content/uploads/2017/06/kotlin.jpg?fit=1920%2C1080&ssl=1)

---

## Tutorial

---

### Print

How can I print an integer entered by an user in Kotlin using scanner?

```kotlin
import java.util.Scanner

fun main(args: Array<String>) {

    val reader = Scanner(System.`in`)
    print("Enter a number: ")

    var integer:Int = reader.nextInt()

    println("You entered: $integer")
}
```

The output of this function will be:

```kotlin
Enter a number: 5
You entered: 5
```

How can I print an integer entered by an user in Kotlin without using scanner?

```kotlin
fun main(args: Array<String>) {

    print("Enter a number: ")

    val stringInput = readLine()!!

    var integer:Int = stringInput.toInt()

    println("You entered: $integer")
}
```

The output of this function will be:

```kotlin
Enter a number: 5
You entered: 5
```

---

### Calculating integers

How can I can I calculate two integers using Kotlin program?

```kotlin
fun main(args: Array<String>) {

    val num1: Int = 5
    val num2: Int = 15

    val sum = num1 + num2

    println("The sum is: $sum")
}
```

The output of this function will be:

```kotlin
The sum is: 20
```

This function will work for addition, subtraction, multiplication, and division when the sign is changed.

---

### Calculating float

How can I calculate two floats using Kotlin program?

```kotlin
fun main(args: Array<String>) {

    val num1 = 1.5f
    val num2 = 4.0f

    val product = num1 * num2

    println("The product is: $product")
}
```

The output of this function will be:

```kotlin
The product is: 6.0
```
