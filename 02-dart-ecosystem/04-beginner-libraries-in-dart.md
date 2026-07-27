# Beginner Libraries in Dart

## What is a Library in Dart?

In Dart, a **library** is a collection of pre-written code — such as
functions, classes, and utilities — that you can use in your program
instead of writing everything from scratch.

Libraries are imported using the `import` keyword:

```dart
import 'dart:math';
```

Dart provides many built-in libraries as part of the Dart SDK. These
libraries provide functionality for common tasks such as:

- Mathematical operations
- File handling
- JSON conversion
- Asynchronous programming
- Collections
- Date and time operations

---

## Essential Beginner Libraries

### 1. `dart:core`

```dart
import 'dart:core';
```

The `dart:core` library contains the fundamental building blocks of the
Dart language.

It provides commonly used types, classes, and functions such as:

- `int`
- `double`
- `String`
- `bool`
- `List`
- `Map`
- `Set`
- `Object`
- `print()`

### Special Note

The `dart:core` library is automatically imported into every Dart file.

Therefore, you normally do not need to write this manually:

```dart
import 'dart:core';
```

For example, this code works without explicitly importing `dart:core`:

```dart
void main() {
  String name = 'Mustafa';
  print(name);
}
```

> `dart:core` is the foundation of the Dart language and is available
> automatically in every Dart program.

---

### 2. `dart:math`

```dart
import 'dart:math';
```

The `dart:math` library provides mathematical functions and constants.

It is useful for:

- Square roots
- Powers
- Trigonometric calculations
- Mathematical constants
- Random number generation

Example:

```dart
import 'dart:math';

void main() {
  print(sqrt(25));

  Random random = Random();
  print(random.nextInt(100));
}
```

Commonly used features include:

| Feature | Purpose |
|---------|---------|
| `sqrt()` | Calculate square root |
| `pow()` | Calculate powers |
| `sin()` | Calculate sine |
| `cos()` | Calculate cosine |
| `Random()` | Generate random values |
| `pi` | Mathematical value of π |

---
