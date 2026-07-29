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

### 3. `dart:convert`

```dart
import 'dart:convert';
```

The `dart:convert` library provides tools for converting data between
different formats.

It is especially commonly used for working with **JSON data** from APIs.

Example:

```dart
import 'dart:convert';

void main() {
  String jsonData = '{"name": "Mustafa", "age": 20}';

  Map<String, dynamic> user = jsonDecode(jsonData);

  print(user['name']);
}
```

You can also convert Dart objects into JSON-compatible strings:

```dart
import 'dart:convert';

void main() {
  Map<String, dynamic> user = {
    'name': 'Mustafa',
    'age': 20,
  };

  String jsonData = jsonEncode(user);

  print(jsonData);
}
```

Commonly used functions include:

| Function | Purpose |
|----------|---------|
| `jsonDecode()` | Convert JSON text into Dart objects |
| `jsonEncode()` | Convert Dart objects into JSON text |

> `dart:convert` is commonly used when communicating with APIs and
> processing structured data.

---

### 4. `dart:io`

```dart
import 'dart:io';
```

The `dart:io` library provides APIs for interacting with the operating
system and the input/output system.

It can be used for:

- Reading files
- Writing files
- Working with directories
- Console input and output
- Sockets
- Other operating-system-level functionality

Example:

```dart
import 'dart:io';

void main() {
  stdout.write('Enter your name: ');

  String? name = stdin.readLineSync();

  print('Hello, $name!');
}
```

It can also be used for file handling:

```dart
import 'dart:io';

void main() {
  File file = File('example.txt');

  file.writeAsStringSync('Hello from Dart!');

  String content = file.readAsStringSync();

  print(content);
}
```

> `dart:io` is commonly used in command-line tools, scripts, backend
> applications, and Dart applications that need direct operating-system
> access.

### Important Note

`dart:io` is not available in every Dart environment.

For example, it cannot be used in Dart web applications because web
applications run inside a browser environment with different security
restrictions.

---

### 5. `dart:async`

```dart
import 'dart:async';
```

The `dart:async` library provides tools for asynchronous programming.

It is commonly used with:

- `Future`
- `Stream`
- `Timer`

Example using `Future`:

```dart
import 'dart:async';

void main() async {
  await Future.delayed(Duration(seconds: 2));

  print('Task completed!');
}
```

Example using `Timer`:

```dart
import 'dart:async';

void main() {
  Timer(Duration(seconds: 2), () {
    print('Timer finished!');
  });
}
```

Example using a `Stream`:

```dart
import 'dart:async';

void main() {
  Stream<int> numbers = Stream.fromIterable([1, 2, 3, 4, 5]);

  numbers.listen((number) {
    print(number);
  });
}
```

> Asynchronous programming is an important part of Dart and Flutter
> development. `Future`, `Stream`, and `async`/`await` will be explored
> in more detail in later sections.

---

## Import Organization in Dart

Dart allows imports to be written in different orders. However, Dart
and Flutter projects commonly follow a consistent organization style
to make code easier to read and maintain.

A common convention is:

```text
1. Dart SDK libraries
2. External packages
3. Project files
```

---

### 1. Dart SDK Libraries

These use the `dart:` prefix:

```dart
import 'dart:async';
import 'dart:convert';
import 'dart:math';
```

---

### 2. External Packages

These are packages added through `pubspec.yaml`.

They use the `package:` prefix:

```dart
import 'package:flutter/material.dart';
import 'package:http/http.dart' as http;
```

---

### 3. Project Files

These are files from your own project:

```dart
import 'models/user_model.dart';
import 'services/api_service.dart';
import 'widgets/custom_button.dart';
```

---

### Example — Organized Imports

```dart
// 1. Dart SDK libraries
import 'dart:async';
import 'dart:convert';

// 2. External packages
import 'package:flutter/material.dart';
import 'package:http/http.dart' as http;

// 3. Project files
import 'models/user_model.dart';
import 'services/api_service.dart';
import 'widgets/custom_button.dart';
```

> Import organization is mainly a code organization convention. The Dart
> compiler does not require imports to be written in this exact order.

---

## Quick Reference Table

| Library | Main Purpose |
|---------|--------------|
| `dart:core` | Fundamental Dart types and functions |
| `dart:math` | Mathematical operations and random numbers |
| `dart:convert` | JSON and data conversion |
| `dart:io` | Files, directories, console I/O, and OS interaction |
| `dart:async` | `Future`, `Stream`, and asynchronous operations |

---

## Quick Recap

> - A **library** is a collection of reusable code.
> - Libraries are imported using the `import` keyword.
> - **`dart:core`** → fundamental Dart types and functions; automatically imported.
> - **`dart:math`** → mathematical operations and random numbers.
> - **`dart:convert`** → JSON and data conversion.
> - **`dart:io`** → file handling, console I/O, and operating-system interaction.
> - **`dart:async`** → `Future`, `Stream`, and asynchronous programming.
> - A common import organization is:
>
>   `dart:` libraries → `package:` libraries → project files
