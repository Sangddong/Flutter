### 1. 변수 선언
**1. var**
```dart
void main () {
  var name = '기존 이름';

  // ❌ 재선언 불가능
  var name = '재선언 이름'; -> Error: 'name' is already declared in this scope.

  // ✅ 재할당 가능
  name = '재할당 이름';
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
---
