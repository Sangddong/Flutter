---
### 1. 변수 선언
**1. var**
```dart
void main () {
  var a = 'this is string';

  // ✅ 재할당 가능
  a = 'another string';

  // ❌ 타입 변경 불가능
  a = 10; -> Error: A value of type 'int' can't be assigned to a variable of type 'String'.
}
```
**2. final**
```dart
void main() {
  final name = '기존 이름';

  // ❌ 재할당 불가능
  name = '재할당 이름'; -> Error: Can't assign to the final variable 'name'.
}
```
**3. const**
```dart
void main() {
  const name = '기존 이름';

  // ❌ 재할당 불가능
  name = '재할당 이름'; -> Error: Can't assign to the const variable 'name'.
}
```
**4. dynamic**
```dart
void main() {
  dynamic a = 'this is string';
  print(a);

  // ✅ 재할당 가능
  a = 'another string';
  print(a);

  // ✅ 타입 변경 가능
  a = 10;
  print(a);
}
```
---
### 2. 타입
1. int
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
2. double
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
3. String
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
4. bool
```dart
void main() {
  bool isTrue = true;
  bool isFalse = false;
  
  print(isTrue);  \\ true
  print(isFalse);  \\ true
}
```
5. 
6. DateTime
