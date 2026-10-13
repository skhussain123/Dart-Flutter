

### Dart Loops
In Programming, loops are used to repeat a block of code until certain conditions are not completed. For, e.g., if you want to print your name 100 times, then rather than typing print(“your name”); 100 times, you can use a loop.

##### There are different types of loop in Dart. They are:

1. For Loop
2. For Each Loop
3. While Loop
4. Do While Loop

```dart
void main() {
  for (int i = 0; i < 10; i++) {
    print("John Doe");
  }
}
```
* Initialization is executed (one time) before the execution of the code block.
* Condition defines the condition for executing the code block.
* Increment/Decrement is executed (every time) after the code block has been executed

```dart
void main() {
  for (int i = 1; i <= 10; i++) {
    print(i);
  }
}
```
```dart
void main(){

  int total = 0;
  int n = 100; // change as per required
  
  for(int i=1; i<=n; i++){
    total = total + i;
  }
  
  print("Total is $total");
  
}
```
```dart
void main(){
  for(int i=50; i<=100; i++){
    if(i%2 == 0){
      print(i);
    }
  } 
}
```

### For Each Loop
The for each loop iterates over all list elements or variables. It is useful when you want to loop through list/collection. The syntax of for-each loop is: 
```dart
void main(){
  List<int> numbers = [1,2,3,4,5];
  
  int total = 0;
  
   numbers.forEach( (num)=>total= total+ num);
  
  print("Total is $total.");
  
  double avg = total / (numbers.length);
  
  print("Average is $avg.");
  
}
```

### For In Loop In Dart
```dart
void main(){
    List<String> footballplayers=['Ronaldo','Messi','Neymar','Hazard'];

  for(String player in footballplayers){
    print(player);
  }
}
```

#### How to Find Index Value Of List
In dart, asMap method converts the list to a map where the keys are the index and values are the element at the index.

```dart
void main(){

List<String> footballplayers=['Ronaldo','Messi','Neymar','Hazard'];

footballplayers.asMap().forEach((index, value) => print("$value index is $index"));

}
```

```dart
void main(){
  
String name = "John";
     
for(var codePoint in name.runes){
  print("Unicode of ${String.fromCharCode(codePoint)} is $codePoint.");
}
}
```

### While Loop
In while loop, the loop’s body will run until and unless the condition is true. You must write conditions first before statements. This loop checks conditions on every iteration. If the condition is true, the code inside {} is executed, if the condition is false, then the loop stops

```dart
void main() {
  int i = 1;
  while (i <= 10) {
    print(i);
    i++;
  }
}
```

```dart
void main(){

  int total = 0;
  int n = 100; // change as per required
  int i =1;

  while(i<=n){
    total = total + i;
    i++;
  }
  
  print("Total is $total");
  
}
```

```dart
void main(){
  int i = 50;
  while(i<=100){
  if(i%2 == 0){
      print(i);
    }
    i++;
  }
}
```

### Do While Loop
Do while loop is used to run a block of code multiple times. The loop’s body will be executed first, and then the condition is tested. The syntax of do while loop is: 

```dart
void main() {
  int i = 1;
  do {
    print(i);
    i++;
  } while (i <= 10);
}
```

```dart
void main(){

  int total = 0;
  int n = 100; // change as per required
  int i =1;
  
  do{
  total = total + i;
    i++;
  }while(i<=n);
  
  print("Total is $total");
  
}
```

### Dart Break and Continue
In this tutorial, you will learn about the break and continue in dart. While working on loops, we need to skip some elements or terminate the loop immediately without checking the condition. In such a situation, you can use the break and continue statement.


#### Break Statement
Sometimes you will need to break out of the loop immediately without checking the condition. You can do this using break statement.

The break statement is used to exit a loop. It stops the loop immediately, and the program’s control moves outside the loop. Here is syntax of break:

```dart
void main() {
  for (int i = 1; i <= 10; i++) {
    if (i == 5) {
      break;
    }
    print(i);
  }
}
```

#### Continue Statement
Sometimes you will need to skip an iteration for a specific condition. You can do this utilizing continue statement.

The continue statement skips the current iteration of a loop. It will bypass the statement of the loop. It does not terminate the loop but rather continues with the next iteration. Here is the syntax of continue statement:

```dart
void main() {
  for (int i = 10; i >= 1; i--) {
    if (i == 4) {
      continue;
    }
    print(i);
  }
}
```

### Exception In Dart
An exception is an error that occurs at runtime during program execution. When the exception occurs, the flow of the program is interrupted, and the program terminates abnormally. There is a high chance of crashing or terminating the program when an exception occurs. Therefore, to save your program from crashing, you need to catch the exception.

```dart
void main() {   
   int a = 18;   
   int b = 0;   
   int res;    
     
   try {    
      res = a ~/ b;
      print("Result is $res");   
   }    
    // It returns the built-in exception related to the occurring exception  
   catch(ex) {   
      print(ex);   
    }   
}  
```

#### Finally In Dart Try Catch
In this example, you will see how to handle the exception using the try-catch block with the finally block.

```dart
void main() {
  int a = 12;
  int b = 0;
  int res;
  try {
    res = a ~/ b;
  } on UnsupportedError {
    print('Cannot divide by zero');
  } catch (ex) {
    print(ex);
  } finally {
    print('Finally block always executed');
  }
}
```

#### Throwing An Exception
In this example, you will see how to throw an exception using the throw keyword.

```dart
void main() {
  try {
    check_account(-10);
  } catch (e) {
    print('The account cannot be negative');
  }
}

void check_account(int amount) {
  if (amount < 0) {
    throw new FormatException(); // Raising explanation externally
  }
}
```

