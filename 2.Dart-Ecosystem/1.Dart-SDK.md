# Dart SDK

## What is the Dart SDK?

The **Dart SDK (Software Development Kit)** is the official collection
of tools, libraries, and utilities used to develop Dart applications.

It provides the tools needed to write, run, analyze, test, and compile
Dart code.

The Dart SDK is also an important part of the Flutter ecosystem. Flutter
includes a compatible Dart SDK with its distribution, allowing developers
to use Dart when building Flutter applications.

> Think of the Dart SDK as the toolkit for the Dart programming language.
> Flutter is a framework built around Dart for creating applications across
> multiple platforms.

---

## What's Inside the Dart SDK?

| Component | Purpose |
|-----------|---------|
| **`dart` command-line tool** | Used to run, compile, analyze, format, test, and manage Dart projects from the terminal |
| **Dart VM** | Executes Dart code during development and supports features such as Just-In-Time (JIT) compilation |
| **Dart Compilers** | Compile Dart code for different targets, including JavaScript, WebAssembly, and native machine code |
| **Pub Package Manager** | Manages external packages and dependencies used by Dart projects |
| **Core Libraries** | Built-in libraries such as `dart:core`, `dart:math`, `dart:async`, and `dart:convert` |
| **Dart Analyzer** | Performs static analysis and detects errors, warnings, and other code issues |
| **dart format** | Automatically formats Dart code according to standard Dart formatting conventions |
| **Dart Documentation Tools** | Generate API documentation from Dart source code and documentation comments |

---

## Dart SDK and Flutter

If you are developing Flutter applications, you generally do **not need
to install the Dart SDK separately**.

The Flutter SDK includes a compatible Dart SDK, which allows Flutter
projects to use Dart for application development.

```text
Flutter SDK
│
├── Flutter Framework
├── Flutter Tools
└── Dart SDK
```

You can use Dart directly through Flutter's bundled SDK:

```bash
dart --version
```

You can also check both the Flutter version and the bundled Dart version:

```bash
flutter --version
```

> The Dart version bundled with Flutter depends on the Flutter SDK version.
> Therefore, the Dart version used by a Flutter project may differ from
> the latest standalone Dart SDK release.

---

## When Do You Need the Standalone Dart SDK?

You may install the standalone Dart SDK when you want to work with Dart
without installing the Flutter SDK.

For example:

- Writing pure Dart programs and scripts
- Building command-line applications
- Developing Dart backend applications
- Creating Dart packages and libraries
- Using Dart tools independently of Flutter

Dart can also be used for server-side development with Dart packages and
frameworks.

---

## Checking Your Dart SDK Version

Once Dart is available on your system, you can check the installed
version using:

```bash
dart --version
```

Example:

```text
Dart SDK version: 3.x.x (stable)
```

If you are using Flutter, you can check the Flutter SDK and its bundled
Dart SDK version using:

```bash
flutter --version
```

Example:

```text
Flutter 3.x.x • channel stable
Dart 3.x.x
```

---

## Common Dart SDK Commands

| Command | What It Does |
|---------|--------------|
| `dart --version` | Displays the installed Dart SDK version |
| `dart create` | Creates a new Dart project |
| `dart run` | Runs a Dart program or project |
| `dart compile` | Compiles Dart code for a specific target |
| `dart pub get` | Gets the dependencies listed in `pubspec.yaml` |
| `dart pub upgrade` | Resolves and upgrades dependencies within the allowed constraints |
| `dart analyze` | Performs static analysis on Dart code |
| `dart format` | Formats Dart source code |
| `dart test` | Runs tests in a Dart project |

> These commands will be explored in more detail in the
> **Dart CLI Commands** section.

---

## Dart SDK vs Flutter SDK

| Aspect | Dart SDK | Flutter SDK |
|--------|----------|-------------|
| **Primary Purpose** | Develop Dart applications | Develop Flutter applications |
| **Includes** | Dart tools, compiler, VM, libraries, and package tools | Flutter framework, Flutter tools, and a compatible Dart SDK |
| **Can Run Pure Dart Code** | Yes | Yes, through its bundled Dart SDK |
| **Can Build Flutter Apps** | No, by itself | Yes |
| **Main Use Case** | Dart applications, scripts, packages, and server-side development | Cross-platform application development |

> **Important:** The Flutter SDK includes the Dart SDK, but the Dart SDK
> does not include the Flutter SDK.

---

## Quick Recap

> - The **Dart SDK** is the official toolkit for developing Dart applications.
> - It includes tools for running, compiling, analyzing, formatting, and testing Dart code.
> - It provides the **Dart VM**, compilers, package management tools, core libraries, and analyzer.
> - The **Flutter SDK includes a compatible Dart SDK**.
> - A separate Dart SDK installation is useful when working with pure Dart projects without Flutter.
> - Use `dart --version` to check the Dart SDK version.
> - Use `flutter --version` to check the Flutter SDK and its bundled Dart version.
