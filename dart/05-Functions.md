

### Dart Functions

1. No Parameter And No Return Type
2. Parameter And No Return Type
3. No Parameter And Return Type
4. Parameter And Return Type

#### No Parameter & No Return Type
```dart
// writing function outside main function.
void printName(){
  print("My name is Raj Sharma. I am from function.");
}
// this is our main function.
void main(){
  printName();
}
```

#### Function With Parameter And No Return Type
```dart
void add(int num1, int num2){
  int sum = num1 + num2;
   print("The sum is $sum");
}

void main(){
  add(10, 20);
}
```


#### No Parameter & Return Type
```dart
void main() {
// Function With No Parameter & Return Type
  String name = primeMinisterName();
  print("The Name from function is $name.");
}
String primeMinisterName() {
  return "John Doe";
}
```

#### Parameter & Return Type
```dart
// this function add two numbers
int add(int a, int b) {
  int sum = a + b;
  return sum;
}

void main() {
  int num1 = 10;
  int num2 = 20;

  int total = add(num1, num2);
  print("The sum is $total.");
}

```

