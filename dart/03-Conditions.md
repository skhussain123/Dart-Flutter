
### Conditions In Dart
When you write a  computer program, you need to be able to tell the computer what to do in different situations. With conditions, you can control the flow of the dart program. Suppose you need to execute a specific code when a particular situation is true. In that case, you can use conditions in Dart. E.g., a calculator app must perform subtraction if the user presses the subtract button and addition if the user taps the add button

#### Types Of Condition
You can use following conditions to control the flow of your program.

* If Condition
* If-Else Condition
* If-Else-If Condition
* Switch case

The easy and most common way of controlling the flow of a program is through the use of an if statement. If statement allow us to execute a code block when the given condition is true. Conditions evaluate boolean values.

### If Condition
```bash
void main()
{
    var age = 20;
    
    if(age >= 18){
      print("You are voter.");
    }
}
```

### If-Else Condition
If the result of the condition is true, then the body of the if-condition is executed. Otherwise, the body of the else-condition is executed.

```dart
void main(){
        int age = 12;
        if(age >= 18){
            print("You are voter.");
        }else{
            print("You are not voter.");
        }
}
```

```dart
void main(){
        bool isMarried = false;
        if(isMarried){
            print("You are married.");
        }else{
            print("You are single.");
        }
}
```

### If-Else-If Condition
When you have multiple if conditions, then you can use if-else-if. You can learn more in the example below. When you have more than two conditions, you can use if, else if, else in dart.

```dart
void main() {
  int noOfMonth = 5;

  // Check the no of month
  if (noOfMonth == 1) {
    print("The month is jan");
  } else if (noOfMonth == 2) {
    print("The month is feb");
  } else if (noOfMonth == 3) {
    print("The month is march");
  } else if (noOfMonth == 4) {
    print("The month is april");
  } else if (noOfMonth == 5) {
    print("The month is may");
  } else if (noOfMonth == 6) {
    print("The month is june");
  } else if (noOfMonth == 7) {
    print("The month is july");
  } else if (noOfMonth == 8) {
    print("The month is aug");
  } else if (noOfMonth == 9) {
    print("The month is sep");
  } else if (noOfMonth == 10) {
    print("The month is oct");
  } else if (noOfMonth == 11) {
    print("The month is nov");
  } else if (noOfMonth == 12) {
    print("The month is dec");
  } else {
    print("Invalid option given.");
  }
}
```

```dart
void main(){
        int num1 = 1200;
        int num2 = 1000;
        int num3 = 150;

        if(num1 > num2  && num1 > num3){
            print("Num 1 is greater: i.e $num1");
        }
        if(num2 > num1 && num2 > num3){
           print("Num2 is greater: i.e $num2");
        }
        if(num3 > num1 && num3 > num2){
            print("Num3 is greater: i.e $num3");
        }
}
```

### Assert
While coding, it is hard to find errors in big projects, so dart provide a assert method to check for the error. It takes conditions as an argument. If the condition is true, nothing happens. If a condition is false, it will raise an error

```dart
void main() { 
   var age = 22;
   assert(age!=22, "Your custom message");
}
```

### How to Run File In Assert Mode
Use this command to run the dart file, which enables assert. If you don’t use this, you will not be able to see the issue. You can use this command below if you are running a dart file from the

```dart
dart --enable-asserts file_name.dart
```


### Switch Case In Dart
In this tutorial, you will learn to use dart switch case to control your program’s flow. A Switch case is used to execute the code block based on the condition

```dart
void main(){
   var dayOfWeek = 5;
if (dayOfWeek == 1) {
        print("Day is Sunday.");
  }
else if (dayOfWeek == 2) {
       print("Day is Monday.");
     }
else if (dayOfWeek == 3) {
      print("Day is Tuesday.");
     }
else if (dayOfWeek == 4) {
        print("Day is Wednesday.");
     }
else if (dayOfWeek == 5) {
        print("Day is Thursday.");
   }
else if (dayOfWeek == 6) {
        print("Day is Friday.");
    }
else if (dayOfWeek == 7) {
        print("Day is Saturday.");
}else{
        print("Invalid Weekday.");
     }
}
```

```dart
void main() {
 const weather = "cloudy";

  switch (weather) {
    case "sunny":
        print("Its a sunny day. Put sunscreen.");
        break;
    case "snowy":
        print("Get your skis.");
      break;
    case "cloudy":
    case "rainy": 
      print("Please bring umbrella.");
      break;
    default:
        print("Sorry I am not familiar with such weather.");
      break;
  }
}
```

#### Switch Case on Enum
Enum (Enumeration) ka istemal apni zaroorat ke mutabiq values define karne ke liye hota hai. Is mein aap apni khud ki ek type bana sakte hain, jismein options ki tadaad pehle se muqarrar hoti hai.
Enum ki madad se aap kisi variable ke liye sirf muqarrar options define kar sakte hain.

```dart
// define enum outside main function
enum Weather{ sunny, snowy, cloudy, rainy}
// main method
void main() {
 const weather = Weather.cloudy;
  
  switch (weather) {
    case Weather.sunny:
        print("Its a sunny day. Put sunscreen.");
        break;
    case Weather.snowy:
        print("Get your skis.");
      break;
    case Weather.rainy:
    case Weather.cloudy:
      print("Please bring umbrella.");
      break;
    default:
        print("Sorry I am not familiar with such weather.");
      break;
  }
}
```

