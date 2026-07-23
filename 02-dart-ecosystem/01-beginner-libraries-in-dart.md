# Beginner Libraries in Dart

## What is a Library in Dart?
In Dart, a **library** is a collection of pre-written code — functions,
classes, and utilities — that you can import into your file to use
their functionality, instead of writing everything from scratch.

Dart libraries are imported using the `import` keyword at the top of
a file:

```dart
import 'dart:core';
```

---

## Essential Beginner Libraries

### 1. `dart:core`
```dart
import 'dart:core';
```
This library contains fundamental building blocks of Dart —
**`print`, `int`, `String`, `List`**, and many other core types and
functions.

> **Special Note:** `dart:core` is **automatically included** in every
> Dart file — you never actually need to write this import statement
> manually. It's there by default.

---

### 2. `dart:math`
```dart
import 'dart:math';
```
Used when you need to perform **mathematical operations**, such as:
- Calculating square roots (`sqrt()`)
- Trigonometric functions (`sin()`, `cos()`)
- Generating random numbers (`Random()`)

---

### 3. `dart:convert`
```dart
import 'dart:convert';
```
Used when you're fetching data from the **internet (APIs)** and need
to convert it into/from **JSON format** — extremely common when
working with REST APIs in Flutter apps.

---

### 4. `dart:io`
```dart
import 'dart:io';
```
Used for **reading and writing files**, and for taking **user input
from the console**. This is one of the **most commonly used**
libraries in real-world Dart applications, especially for command-line
tools and backend scripts.

---

### 5. `dart:async`
```dart
import 'dart:async';
```
Used for working with **`Future`** and **`Streams`** — essential when
a task needs to complete **after some delay** or when handling
asynchronous operations (like network requests or timers).

---

## Import Sequence in Dart
Unlike languages like C++, where you can write header imports (like
`#include <iostream>` or `#include <cmath>`) in **any order** without
issue — because C++ typically runs synchronously and the compiler has
time to fetch each library one operation at a time — **Dart has a
specific, recommended sequence** for organizing imports.

This sequence isn't overly complicated, and following it keeps your
code clean and consistent:

### Recommended Import Order

1. **Dart core libraries first** (`dart:` prefix)
```dart
   import 'dart:core';
   import 'dart:math';
   import 'dart:async';
```

2. **External packages next** (`package:` prefix — things installed
   via `pubspec.yaml`, including Flutter's own packages)
```dart
   import 'package:flutter/material.dart';
   import 'package:http/http.dart';
```

3. **Your own project files last** (relative imports)
```dart
   import 'models/user_model.dart';
   import 'services/api_service.dart';
```

### Example — Correct Import Order

```dart
// 1. Dart core libraries
import 'dart:async';
import 'dart:convert';

// 2. External packages
import 'package:flutter/material.dart';
import 'package:http/http.dart' as http;

// 3. Your own project files
import 'models/user_model.dart';
import 'widgets/custom_button.dart';
```

> Following this order isn't strictly enforced by the Dart compiler
> (your code will still run if you mix the order), but it's a widely
> followed **best practice** in the Dart/Flutter community for
> readability and maintainability. Many linters (like `flutter_lints`)
> will actually warn you if your imports aren't properly ordered.

---

## Quick Recap
> - Libraries are imported using the `import` keyword
> - **`dart:core`** → automatic, no need to import manually
> - **`dart:math`** → mathematical operations
> - **`dart:convert`** → JSON conversion (APIs)
> - **`dart:io`** → file handling & console input (most used)
> - **`dart:async`** → `Future` and `Stream` for async operations
> - **Import order:** `dart:` libraries → `package:` libraries → your
>   own project files
