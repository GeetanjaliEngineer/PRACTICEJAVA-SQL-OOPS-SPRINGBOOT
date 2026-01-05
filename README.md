# PRACTICEJAVA-SQL-OOPS-SPRINGBOOT

This repository contains **Core Java practice programs**, covering **loops, patterns, arrays, strings, OOP concepts**, and basic **logic-building questions**. It is useful for beginners and interview preparation.

---

## 📌 Star Pattern Programs

### 1️⃣ Right Angle Star Triangle

```
*
**
***
****
*****
```

```java
for(int i = 1; i <= 5; i++){
    for(int j = 1; j <= i; j++){
        System.out.print("* ");
    }
    System.out.println();
}
```

---

### 2️⃣ Number Triangle

```
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5
```

```java
for(int i = 1; i <= 5; i++){
    for(int j = 1; j <= i; j++){
        System.out.print(j + " ");
    }
    System.out.println();
}
```

---

### 3️⃣ Pyramid Star Pattern

```
    *
   ***
  *****
 *******
*********
```

```java
int rows = 5;
for(int i = 1; i <= rows; i++){
    for(int j = 1; j <= rows - i; j++){
        System.out.print(" ");
    }
    for(int k = 1; k <= (2 * i - 1); k++){
        System.out.print("*");
    }
    System.out.println();
}
```

---

### 4️⃣ Inverted Pyramid

```
*********
 *******
  *****
   ***
    *
```

```java
int rows = 5;
for(int i = rows; i >= 1; i--){
    for(int j = 1; j <= rows - i; j++){
        System.out.print(" ");
    }
    for(int k = 1; k <= (2 * i - 1); k++){
        System.out.print("*");
    }
    System.out.println();
}
```

---

## 🔢 Loop & Number Programs

### ✔ Print Even Numbers (2–20)

```java
for(int i = 2; i <= 20; i++){
    if(i % 2 == 0)
        System.out.println(i);
}
```

### ✔ Sum of First 5 Numbers

```java
int sum = 0;
for(int i = 1; i <= 5; i++){
    sum += i;
}
System.out.println("Sum = " + sum);
```

### ✔ Print "Java" 10 Times

```java
for(int i = 1; i <= 10; i++){
    System.out.println("Java");
}
```

### ✔ Print Odd Numbers (1–15)

```java
for(int i = 1; i <= 15; i++){
    if(i % 2 != 0)
        System.out.println(i);
}
```

---

## 🧮 Factorial Program

```java
int factorial = 1;
for(int i = 1; i <= 5; i++){
    factorial *= i;
}
System.out.println("Factorial = " + factorial);
```

---

## 🔁 Reverse a Number

```java
int num = 123;
int rev = 0;
while(num != 0){
    int digit = num % 10;
    rev = rev * 10 + digit;
    num /= 10;
}
System.out.println("Reverse number = " + rev);
```

---

## 🔍 Prime Number Check

```java
int n = 17;
boolean isPrime = true;

for(int i = 2; i <= n / 2; i++){
    if(n % i == 0){
        isPrime = false;
        break;
    }
}

if(isPrime)
    System.out.println(n + " is Prime");
else
    System.out.println(n + " is Not Prime");
```

---

## 📦 Arrays

### ✔ Print Array Elements

```java
int[] arr = {2, 4, 6, 8, 10};
for(int i = 0; i < arr.length; i++){
    System.out.println(arr[i]);
}
```

### ✔ Sum of Array Elements

```java
int sum = 0;
for(int i = 0; i < arr.length; i++){
    sum += arr[i];
}
System.out.println("Sum = " + sum);
```

### ✔ Largest Number in Array

```java
int[] arr = {10, 45, 2, 89, 30};
int max = arr[0];

for(int i = 1; i < arr.length; i++){
    if(arr[i] > max)
        max = arr[i];
}
System.out.println("Largest = " + max);
```

---

## 🔤 Strings

### ✔ Reverse a String

```java
String str = "hello";
String rev = "";

for(int i = str.length() - 1; i >= 0; i--){
    rev += str.charAt(i);
}
System.out.println("Reversed = " + rev);
```

### ✔ Palindrome String Check

```java
String str = "level";
String rev = "";

for(int i = str.length() - 1; i >= 0; i--){
    rev += str.charAt(i);
}

if(str.equals(rev))
    System.out.println("Palindrome");
else
    System.out.println("Not Palindrome");
```

### ✔ Print Each Character of String

```java
String str = "Java";
for(int i = 0; i < str.length(); i++){
    System.out.println(str.charAt(i));
}
```

---

## 🧠 OOPS Concept – Encapsulation

```java
class Student{
    private int id;
    private String name;

    public void setId(int id){
        this.id = id;
    }
    public int getId(){
        return id;
    }
    public void setName(String name){
        this.name = name;
    }
    public String getName(){
        return name;
    }
}
```

```java
public class Test{
    public static void main(String[] args){
        Student s = new Student();
        s.setId(1);
        s.setName("Geetanjali");

        System.out.println(s.getId());
        System.out.println(s.getName());
    }
}
```

---

## 🚀 Tech Stack

* Core Java
* OOP Concepts
* Logic Building
* SQL (Upcoming)
* Spring Boot REST APIs (Upcoming)

---

✨ *This repository is for daily practice and interview preparation.*
