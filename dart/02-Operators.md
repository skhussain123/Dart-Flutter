

### Operators In Dart
Operators are used to perform mathematical and logical operations on the variables. Each operation in dart uses a symbol called the operator to denote the type of operation it performs. Before learning operators in the dart, you must understand the following things.


##### There are different types of operators in dart. They are as follows:
1. Arithmetic Operators
2. Increment and Decrement Operators
3. Assignment Operators
4. Logical Operators
5. Type Test Operators

#### Arithmetic operators
Arithmetic operators are the most common types of operators. They perform operations like addition, subtraction, multiplication, division, etc

| Operator Symbol | Operator Name    | Description                                                                |
| --------------- | ---------------- | -------------------------------------------------------------------------- |
| `+`             | Addition         | Do operands ko add karne ke liye use hota hai.                             |
| `-`             | Subtraction      | Do operands ko subtract karne ke liye use hota hai.                        |
| `-expr`         | Unary Minus      | Expression ka sign reverse karne ke liye use hota hai.                     |
| `*`             | Multiplication   | Do operands ko multiply karne ke liye use hota hai.                        |
| `/`             | Division         | Do operands ko divide karta hai aur result `double` mein deta hai.         |
| `~/`            | Integer Division | Division ka integer result deta hai, decimal part ko discard kar deta hai. |
| `%`             | Modulus          | Division ke baad remainder (baqi) deta hai.                                |

```dart
void main() {
 // declaring two numbers 
 int num1=10;
 int num2=3;
 
 // performing arithmetic calculation
 int sum=num1+num2;       // addition
 int diff=num1-num2;      // subtraction
 int unaryMinus = -num1;    // unary minus  
 int mul=num1*num2;       // multiplication
 double div=num1/num2;    // division
 int div2 =num1~/num2;     // integer division
 int mod=num1%num2;       // show remainder
 
//Printing info 
 print("The addition is $sum.");
 print("The subtraction is $diff.");
 print("The unary minus is $unaryMinus.");
 print("The multiplication is $mul.");
 print("The division is $div.");
 print("The integer division is $div2.");
 print("The modulus is $mod."); 
}
```


### Increment and Decrement Operators
Increment aur decrement operators variable ki value ko 1 se increase ya decrease karte hain. `++` ya `--` agar variable se pehle ho to prefix kehlata hai, aur baad mein ho to postfix.

| Operator Symbol | Operator Name  | Description                                                                                    |
| --------------- | -------------- | ---------------------------------------------------------------------------------------------- |
| `++var`         | Pre Increment  | Value ko 1 se increase karta hai. `var = var + 1`. Expression ki value updated value hoti hai. |
| `--var`         | Pre Decrement  | Value ko 1 se decrease karta hai. `var = var - 1`. Expression ki value updated value hoti hai. |
| `var++`         | Post Increment | Value ko 1 se increase karta hai. `var = var + 1`. Expression ki value purani value hoti hai.  |
| `var--`         | Post Decrement | Value ko 1 se decrease karta hai. `var = var - 1`. Expression ki value purani value hoti hai.  |


```dart
void main() {
// declaring two numbers 
 int num1=0;
 int num2=0;
 
// performing increment / decrement operator  

// pre increment   
num2 = ++num1;
print("The value of num2 is $num2");

// reset value to 0 
num1 = 0;
num2 = 0;

// post increment  
num2 =  num1++;
print("The value of num2 is $num2"); 
  
}

Output:
The value of num2 is 1
The value of num2 is 0


```

### Assignment Operators
It is used to assign some values to variables. Here, we are assigning 24 to the age variable.

```dart
void main() {
  double age = 24;
  age+= 1;  // Here age+=1 means age = age + 1.
  print("After Addition Age is $age");
  age-= 1;  //Here age-=1 means age = age - 1.
  print("After Subtraction Age is $age");
  age*= 2;  //Here age*=2 means age = age * 2.
  print("After Multiplication Age is $age");
  age/= 2;  //Here age/=2 means age = age / 2.
  print("After Division Age is $age");
}
```

### Relational Operators
Relational operators are also called comparison operators. They are used to make a comparison.

| Operator Symbol | Operator Name            | Description                                                                                           |
| --------------- | ------------------------ | ----------------------------------------------------------------------------------------------------- |
| `>`             | Greater than             | Check karta hai ke pehli value doosri value se bari hai ya nahi. Result `bool` hota hai.              |
| `<`             | Less than                | Check karta hai ke pehli value doosri value se chhoti hai ya nahi. Result `bool` hota hai.            |
| `>=`            | Greater than or equal to | Check karta hai ke pehli value doosri value se bari ya barabar hai ya nahi. Result `bool` hota hai.   |
| `<=`            | Less than or equal to    | Check karta hai ke pehli value doosri value se chhoti ya barabar hai ya nahi. Result `bool` hota hai. |
| `==`            | Equal to                 | Check karta hai ke dono values barabar hain ya nahi. Result `bool` hota hai.                          |
| `!=`            | Not equal to             | Check karta hai ke dono values barabar nahi hain. Result `bool` hota hai.                             |

```dart
void main() {
  
 int num1=10;
 int num2=5;
 //printing info
 print(num1==num2); 
 print(num1<num2);
 print(num1>num2);
 print(num1<=num2);
 print(num1>=num2);
}
```


