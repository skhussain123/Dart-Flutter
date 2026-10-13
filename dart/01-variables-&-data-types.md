


### Types of Variables:
1. String: For storing text value. E.g. “John” [Must be in quotes]
2. int: For storing integer value. E.g. 10, -10, 8555 [Decimal is not included]
3. double: For storing floating point values. E.g. 10.0, -10.2, 85.698 [Decimal is included]
4. num: For storing any type of number. E.g. 10, 20.2, -20 [both int and double]
5. bool: For storing true or false. E.g. true, false [Only stores true or false values]
6. var: For storing any value. E.g. ‘Bimal’, 12, ‘z’, true


### Rules For Creating Variables In Dart
* Rules For Creating Variables In Dart
* Variable names are case sensitive, i.e., a and A are different.
* A variable name can consist of letters and alphabets.
* A variable name cannot start with a number.
* Keywords are not allowed to be used as a variable name.
* Blank spaces are not allowed in a variable name.
* Special characters are not allowed except for the underscore (_) and the dollar ($) sign


```dart
void main() {
// declaring variables
String name = "John";
String address = "USA";  
num age = 20; // used to store any types of numbers 
num height = 5.9;
bool isMarried = false;
   
// printing variables value   
print("Name is $name");
print("Address is $address");
print("Age is $age");
print("Height is $height");
print("Married Status is $isMarried");
}
```

<br>

Constant is the type of variable whose value never changes. In  programming, changeable values are mutable and unchangeable values are immutable. Sometimes, you don’t need to change the value once declared. Like the value of PI=3.14, it never changes. To create a constant in Dart, you can use the const keyword.

```dart
void main(){
const pi = 3.14;
pi = 4.23; // not possible  
print("Value of PI is $pi");
}
```

### Data Types
1. Numbers
2. Strings
3. Booleans
4. Lists
5. Maps
6. Sets
7. Runes
8. Null

### Built-In Types
In Dart language, there is the type of values that can be represented and manipulated. The data type classification is as given below:
<br>

| Data Type | Keyword                | Description                                               |
| --------- | ---------------------- | --------------------------------------------------------- |
| Numbers   | `int`, `double`, `num` | Numeric values ko represent karta hai.                    |
| Strings   | `String`               | Characters aur text ki sequence ko represent karta hai.   |
| Booleans  | `bool`                 | Boolean values `true` aur `false` ko represent karta hai. |
| Lists     | `List`                 | Items ke ordered group ko represent karta hai.            |
| Maps      | `Map`                  | Key-value pairs ki form mein data store karta hai.        |
| Sets      | `Set`                  | Unique values ka collection hota hai.                     |
| Runes     | `runes`                | String ke Unicode code points ko represent karta hai.     |
| Null      | `null`                 | Kisi value ki absence ko represent karta hai.             |



#### Number
When you need to store numeric value on dart, you can use either int or double. Both int and double are subtypes of num. You can use num to store both int or double value.

<br>

```dart
void main() {
// Declaring Variables  
int num1 = 100; // without decimal point.
double num2 = 130.2; // with decimal point.
num num3 = 50;
num  num4 = 50.4;  

// For Sum   
num sum = num1 + num2 + num3 + num4;
   
// Printing Info   
print("Num 1 is $num1");
print("Num 2 is $num2");  
print("Num 3 is $num3");  
print("Num 4 is $num4");  
print("Sum is $sum");  
   
}
```
<br>

#### String 
```dart
void main() {
// Declaring Values     
String schoolName = "Diamond School";
String address = "New York 2140";   

// Printing Values
print("School name is $schoolName and address is $address");   
}
```

##### Special Character In String
* \n New Line
* \t Tab

```dart
void main() {
   
// Using \n and \t   
print("I am from \nUS.");
print("I am from \tUS.");
}
```
##### Create A Raw String In Dart
```dart
// Set price value
num price = 10;
String withoutRawString = "The value of price is \t $price"; // regular String
String withRawString =r"The value of price is \t $price"; // raw String

print("Without Raw: $withoutRawString"); // regular result
print("With Raw: $withRawString"); // with raw result

output:
Without Raw: The value of price is 	 10
With Raw: The value of price is \t $price
```


### Type Conversion In Dart
#### Convert String To Int In Dart
```dart
void main() {
String strvalue = "1";
print("Type of strvalue is ${strvalue.runtimeType}"); 
  
int intvalue = int.parse(strvalue);
print("Value of intvalue is $intvalue");

print("Type of intvalue is ${intvalue.runtimeType}");
}

Output:
Type of strvalue is String
Value of intvalue is 1
Type of intvalue is int

```
##### And more methods for conversion
* Convert String To Double In Dart
* Convert Int To String In Dart
* Convert Double To Int In Dart


### Lists
The list holds multiple values in a single variable. It is also called arrays. If you want to store multiple values without creating multiple variables, you can use a list.

```dart
void main() {
  
List<String> names = ["Raj", "John", "Max"];
print("Value of names is $names");
print("Value of names[0] is ${names[0]}"); // index 0

int length = names.length;  
print("The Length of names is $length");
}

Output:
Value of names is [Raj, John, Max]
Value of names[0] is Raj
The Length of names is 3

```

### Sets
An unordered collection of unique items is called set in dart. You can store unique data in sets.
Set doesn’t print duplicate items.

```dart
void main() {
 
 Set<String> weekday = {"Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"};
 print("Value of names is $weekday");


  int length = weekday.length;
  print("The Length of names is $length");
}

Output:
Value of names is {Sun, Mon, Tue, Wed, Thu, Fri, Sat}
The Length of names is 7
```


### Maps
In Dart, a map is an object where you can store data in key-value pairs. Each key occurs only once, but you can use same value multiple times.

```dart
void main() {
 
 Map<String,String> mydata = {
   'name' : 'hussain', 
   'father' : 'faheem'
   
   };
  print("Value of name is $mydata");
  print(mydata['name']);

}

Output:
Value of names is {name: hussain, father: faheem}
hussain

```

#### Var Keyword In Dart
In Dart, var automatically finds a  data type. In simple terms, var says if you don’t want to specify a data type, I will find a data type for you.

```dart
void main(){

var name = "John Doe"; // String
var age = 20; // int

print(name);
print(age);
}
```

#### Runes In Dart
With runes, you can find Unicode values of String. The Unicode value of a is 97, so runes give 97 as output.
```dart
void main() {

String value = "a";
print(value.runes);
}
```

#### How To Check Runtime Type
You can check runtime type in dart with .runtimeType after the variable name.
```dart
void main() { 
   var a = 10;
   print(a.runtimeType); 
   print(a is int); // true
}
```