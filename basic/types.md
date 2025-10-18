### 2. 타입
**1. int**
```dart
void main() {
  int a = 10;
  int b = 5;
  
  print(a + b);  // 15
  print(a - b);  // 5
  print(a * b);  // 50
  print(a / b);  // 2
}
```
**2. double**
```dart
void main() {
  double a = 10.5;
  double b = 5.0;
  
  print(a + b);  // 15.5
  print(a - b);  // 5.5
  print(a * b);  // 52.5
  print(a / b);  // 2.1
}
```
**3. String**
```dart
void main() {
  String str1 = "";
  String str2 = "hello";
  String str3 = "world!";
  String str4;
  String? str5;

  print(str1);  \\
  print(str2);  \\ hello
  print(str2 + " " + str3); \\ hello world!
  print("$str2 ${str3}");  \\ hello world!
  print(str4) -> Error: Non-nullable variable 'str4' must be assigned before it can be used.
  print(str5)  \\ null
}
```
```dart
void main() {
  String str1 = "apple";
  final String str2 = "banana";
  const String str3 = "grape";

  print(str1); // apple
  print(str2); // banana
  print(str3); // grape

  dynamic String str4 = "error";
}
```
**4. bool**
```dart
void main() {
  bool isTrue = true;
  bool isFalse = false;
  
  print(isTrue);  \\ true
  print(isFalse);  \\ true
}
```
5. DateTime
```dart
void main () async {
  DateTime now1 = DateTime.now();
  await Future.delayed(Duration(seconds: 3));
  DateTime now2 = DateTime.now();
  
  print(now1);  // 2025-10-08 17:46:25.948
  print(now2);  // 2025-10-08 17:46:29.310
}
```

