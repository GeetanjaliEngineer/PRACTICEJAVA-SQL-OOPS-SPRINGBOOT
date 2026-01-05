# PRACTICEJAVA-SQL-OOPS-SPRINGBOOT

public class starPattern(){
	public static void main(String args[]){
		//int a = 5;
		for( int i=1; i<=5; i++){
			for(int j = 1; j<=i ; j++){
				System.out.println("* ");
			}
			System.out.println();

		}
	}
}

*
**
***
****
*****

int a = 5;
for(int i = 1; i<= 5; i++){
	for(int j = 1 ; j<= i; j++) {
		System.out.println(j + " ");
	}
System.out.println();
}
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5 


    *    
   ***
  *****
 *******
*********    
int row =5;
for(int i =1; i<=rows; i++){
	//print spaces
	for(int j=1; j<=rows; j++){
		System.out.print(" "); // double space for alignment
	}
	//print stars
	for(int k =1;k<=(2*i-1) ; k++){
		System.out.println("* ");
	}
	System.out.println(); //next row
}



*********
 *******
  *****
   ***
    *
  int rows = 5;
	for(int i = rows; i >= 1; i--){
    // Print spaces
    for(int j = 1; j <= rows - i; j++){
        System.out.print("  "); // two spaces for alignment
    }
    // Print stars
    for(int k = 1; k <= (2*i - 1); k++){
        System.out.print("* ");
    }
    System.out.println(); // move to next row
}

//outer loop --> i = rows to 1 (reverse)
// spaces --> rows-i;
// Stars --> (2* i -1)
// System.out.println(--same line)
//  System.out.println(same line)



Right angle tringle 
*
**
***
****
*****
******

for( i=1 ; i<= 5; i++){
	for(j =1 ; j<=i ; j++){
		System.out.println("* ");
	}
	System.out.println();
}

1
12
123
1234
12345

for( i=1 ; i<= 5; i++){
	for(j =1 ; j<=i ; j++){
		System.out.println( j + " ");
	}
	System.out.println();
}

        * 
      * * * 
    * * * * * 
  * * * * * * * 
* * * * * * * * * 

int rows = 5;
for(int i= 1;i<=rows; i++){
 for ( int j = 1; j <= rows-i; j++){
 	System.out.println( " ");
 }
 for( int k =1; k<= (2*i-1); k++)
{
	System.out.println("* ");

}
System.out.println();

}
* * * * * * * * * 
  * * * * * * * 
    * * * * * 
      * * * 
        * 
int rows = 5;
for(int i= 1;i>=rows; i++){
 for ( int j = 1; j <= rows-i; j++){
 	System.out.println( " ");
 }
 for( int k =1; k<= (2*i-1); k++)
{
	System.out.println("* ");

}
System.out.println();

}


//print even no. from 2 to 20 using a loop 

public class EvenNumbers {
    public static void main(String[] args) {
        for(int i = 2; i <= 20; i++) { // start from 2
            if(i % 2 == 0) {
                System.out.println(i); // print the current even number
            }
        }
    }
}


//print sum of first 5 numbers 
1 2 3 4 5 

int sum =0;
for(int i=1; i<=5; i++){
	sum += i;
}
System.out.println("Sum =" + sum);

//output =15 




// print " Java " 10 times 
for(int i = 1 ; i<= 10; i++){
	System.out.println("Java");
}

//print odd number from 1 to 15 

for(int i=1; i<=15;i++){
	if(i%2 != 0){
		System.out.println(i);
	}
}

// factorial of 5 
1 2 3 4 5 
5*4*3*2*1= 
5*4=20
20*3= 60 
60* 2 = 120 
120*1 = 120 
// so factorial is 120 

int factorial = 1 ;
for(int i=1 ; i<=5; i++){
	factorial *= i;
}
System.out.println("Factorial =" + factorial );


// output is 120 



//Write a program to reverse a no.
int num =123;
int rev = 0;
while(num != 0){
	int digit = num % 10;
	rev = rev*10+digit;
	num /= 10;
}
System.out.println("reverse no =" + rev);


// output = 321



//check prime no 

int n = 17 ;

boolean isPrime = true;
for( int = 2 ; i<= n/2 ; i++){
	if(n% 1 == 0){
		isPrime = false;
		break;

	}
}
if(isPrime)
	System.out.println(n + " is prime ");
else 
	System.out.println( n + " is not prime no ");











//arrays and strings


//Print all elements of array 
int[] arr = {2,4,6,8,10};
for(int i=0; i<arr.length; i++){
	System.out.println(arr[i]);
}







//Sum of array elements 
int sum =0;
for(int i=0; i<arr.length; i++){
		sum += arr[i];
}
System.out.println("Sum" + sum);
//sum = 30






//Reverse a string 
String str="hello" ;  // reverse this =olleh
String rev="";
for(int i=str.length()-1; i>=0; i--){
	rev += str.charAt(i);

}
System.out.println("Reversed =" +rev);





// check palindrome String (reads same forward and backward)
String str="level";
String rev="";

for(int i=str.length()-1; i>=0; i--){
	rev += str.charAt(i);
}
//check palindrome 
if(str.equals(rev)){
	System.out.println(str + "is palindrome ");

} else {
	System.out.println(str + "is not palindrome ");
}
.// madam is palindrome 







//Create an array {1, 3, 5, 7, 9} → print even numbers only

int[] arr  = {1, 3, 5, 7, 9};
for(int i =0 ; i<arr.length; i++){
	if(arr[i] % 2 == 0){
		System.out.println("even no. " arr[i]);
	}else{
		System.out.println("No even no. array ");
	}
}






//String "Java" → print each character on a new line


// I use the charAt() method to access each character
 // of a string using a loop.
String str ="Java";
for(int i=0; i<str.length();i++){
	System.out.println(str.charAt(i));
}
J
a
v
a



PRACTICE 3 OOPS+CORE JAVA LOGIC QUESTION+SQL +SPRINGBOOT -REST APIS 



OOPs+Logic 

Concept : Encapsulation 
Encapsulation means wrapping data and methods together and hiding data using private access.

class Student{

	//encapuslate this date as using private access modifier 

	private int id;
	private String name;
	
//getter and setter 
	public void setId(int id){
		this.id=id;
	}
	public int getId(){
		return id;
	}
	public void setName(String name){
		this.name=name;

	}
	public String getName(){
		return name;
	}
	public class Test{
		public static void main(String[] args){
			//object 
			Student s = new Student();
			s.setId(1);
			s.setName("Geetanjali");

			System.out.println(s.getId);
			System.out.println(s.getName);

		}
	}
}


Java core logic 

// find the largest number in array 

int[] arr = {10,45,2,89,30};
int max = arr[0];

for(int i =1; i<arr.length; i++){
	if(arr[i]>max){
		max = arr[i];
	}
}
System.out.println("Largest" +max);


