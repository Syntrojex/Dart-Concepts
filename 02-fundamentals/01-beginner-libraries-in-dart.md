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
