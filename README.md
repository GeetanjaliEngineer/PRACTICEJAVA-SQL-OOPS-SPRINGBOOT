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


# PRACTICE 3 – OOPS + Core Java + SQL + Spring Boot REST APIs

This repository contains **basic interview-oriented practice** for:

* OOPS (Encapsulation)
* Core Java logic questions
* SQL queries
* Spring Boot REST APIs

---

## 🔹 OOPS + Logic

### Concept: Encapsulation

Encapsulation means **wrapping data (variables) and methods together** and **hiding data** using the `private` access modifier.

### Example: `Student` Class

```java
class Student {

    // encapsulated data using private access modifier
    private int id;
    private String name;

    // getters and setters
    public void setId(int id) {
        this.id = id;
    }

    public int getId() {
        return id;
    }

    public void setName(String name) {
        this.name = name;
    }

    public String getName() {
        return name;
    }
}

class Test {
    public static void main(String[] args) {
        // object creation
        Student s = new Student();
        s.setId(1);
        s.setName("Geetanjali");

        System.out.println(s.getId());
        System.out.println(s.getName());
    }
}
```

---

## 🔹 Core Java Logic

### Find the Largest Number in an Array

```java
int[] arr = {10, 45, 2, 89, 30};
int max = arr[0];

for (int i = 1; i < arr.length; i++) {
    if (arr[i] > max) {
        max = arr[i];
    }
}

System.out.println("Largest number: " + max);
```

---

## 🔹 SQL Practice

### 1. Create Table

```sql
CREATE TABLE employee (
    id INT PRIMARY KEY,
    name VARCHAR(50),
    salary INT,
    department VARCHAR(30)
);
```

### 2. Insert Data

```sql
INSERT INTO employee VALUES (1, 'John', 40000, 'IT');
INSERT INTO employee VALUES (2, 'Aman', 30000, 'HR');
```

### 3. Important Interview Queries

```sql
SELECT * FROM employee;

SELECT name, salary FROM employee;

SELECT * FROM employee WHERE salary > 35000;

SELECT * FROM employee ORDER BY salary DESC;
```

### Difference Between `WHERE` and `HAVING`

* **WHERE**: Filters rows **before** `GROUP BY`
* **HAVING**: Filters records **after** `GROUP BY`

---

## 🔹 Spring Boot – REST APIs

### 1. Simple REST Controller

```java
@RestController
@RequestMapping("/api")
public class TestController {

    @GetMapping("/hello")
    public String hello() {
        return "Hello from Spring Boot";
    }
}
```

---

### 2. REST API for Student

```java
@RestController
@RequestMapping("/student")
public class StudentController {

    @GetMapping("/{name}")
    public String getStudent(@PathVariable String name) {
        return "Student name is " + name;
    }
}
```

### Sample URL

```
http://localhost:8080/student/John
```

---

## 🔹 Mini Practice

### Java: `Employee` Class (Encapsulation)

```java
class Employee {
    private int id;
    private String employeeName;

    public void setId(int id) {
        this.id = id;
    }

    public int getId() {
        return id;
    }

    public void setEmployeeName(String employeeName) {
        this.employeeName = employeeName;
    }

    public String getEmployeeName() {
        return employeeName;
    }
}

class EmployeeTest {
    public static void main(String[] args) {
        Employee emp = new Employee();
        emp.setId(1);
        emp.setEmployeeName("Riya");

        System.out.println(emp.getId());
        System.out.println(emp.getEmployeeName());
    }
}
```

**Output:**

```
1
Riya
```

---

### SQL: Get Highest Salary

```sql
SELECT MAX(salary) FROM employee;
```

---

### Spring Boot: `/api/welcome` GET API

```java
@RestController
@RequestMapping("/api")
public class WelcomeController {

    @GetMapping("/welcome")
    public String welcome() {
        return "Hello from Spring Boot";
    }
}
# 🚀 Java • SQL • Spring Boot Practice

This repository contains my **daily practice** covering **Core Java logic**, **SQL queries**, and **Spring Boot REST APIs**. It is structured to strengthen fundamentals required for a **Java Developer** role.

---

## 🟢 Core Java Practice

### ✅ Count Vowels in a String

```java
String str = "Geetanjali";
int count = 0;

for (int i = 0; i < str.length(); i++) {
    char ch = str.charAt(i);
    if (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u'
            || ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U') {
        count++;
    }
}
System.out.println("Vowels count = " + count);
```

**Explanation:**

* Traversed the string character by character
* Checked vowels using conditional statements

---

### ✅ Count Consonants in a String

```java
String str = "Roshni";
int count = 0;

for (int i = 0; i < str.length(); i++) {
    char ch = str.charAt(i);
    if (Character.isLetter(ch) &&
        !(ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u'
        || ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U')) {
        count++;
    }
}
System.out.println("Consonants count = " + count);
```

---

## 🟣 SQL Practice

### 1️⃣ Find Highest Salary

```sql
SELECT MAX(salary) FROM employees;
```

### 2️⃣ Find Second Highest Salary

```sql
SELECT MAX(salary)
FROM employees
WHERE salary < (SELECT MAX(salary) FROM employees);
```

### 3️⃣ Count Employees Department-wise

```sql
SELECT department, COUNT(*)
FROM employees
GROUP BY department;
```

### ❓ What is GROUP BY?

`GROUP BY` groups rows that have the same values in specified columns and is commonly used with aggregate functions like `COUNT`, `SUM`, `AVG`, `MAX`, and `MIN`.

---

### 4️⃣ Employee with Minimum Salary

```sql
SELECT *
FROM employees
WHERE salary = (SELECT MIN(salary) FROM employees);
```

**Explanation:**

* Used a subquery to fetch the minimum salary
* Retrieved complete employee details

---

## 🔵 Spring Boot – REST API (CRUD Start)

### 📌 Entity

```java
@Entity
public class Employee {

    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private int id;
    private String name;
    private int salary;

    // Getters and Setters
}
```

---

### 📌 Repository

```java
public interface EmployeeRepository extends JpaRepository<Employee, Integer> {
}
```

---

### 📌 Controller (GET + POST)

```java
@RestController
@RequestMapping("/employees")
public class EmployeeController {

    @Autowired
    private EmployeeRepository repo;

    @GetMapping
    public List<Employee> getAll() {
        return repo.findAll();
    }

    @PostMapping
    public Employee save(@RequestBody Employee emp) {
        return repo.save(emp);
    }
}
```

---

### 📌 GET Employee by ID API

```java
@GetMapping("/{id}")
public Employee getEmployeeByID(@PathVariable int id) {
    return repo.findById(id).orElse(null);
}
```

**URL:**

```
GET http://localhost:8888/employees/1
```

**Explanation:**

* Fetches employee data using ID
* Uses Spring Data JPA `findById()` method

---

## ✨ Tech Stack

* Java (Core + OOP)
* SQL
* Spring Boot
* Spring Data JPA
* REST APIs

---

📌 *This repository reflects my continuous learning and hands-on practice toward becoming a strong Java Backend Developer.* 💪
