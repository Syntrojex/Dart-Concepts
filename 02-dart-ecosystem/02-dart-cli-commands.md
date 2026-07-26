# Dart CLI / Terminal Commands

## What is the Dart CLI?

The `dart` command-line tool is the command-line interface for the Dart
SDK.

It is available whether you install Dart through the standalone Dart SDK
or use the Dart SDK bundled with Flutter.

The Dart CLI provides a single interface for common development tasks,
including:

- Running Dart programs
- Creating projects
- Analyzing code
- Formatting code
- Managing packages
- Running tests
- Generating documentation
- Compiling Dart applications

> The `dart` command is the main way to interact with the Dart SDK from
> the terminal.

---

## 1. `dart run`

Runs a Dart program from the terminal.

```bash
dart run main.dart
```

For a Dart project, you can also run the project's main executable:

```bash
dart run
```

---

## 2. `dart analyze`

Analyzes Dart code for errors, warnings, and other diagnostics using
static analysis.

The analysis performed by `dart analyze` is the same type of analysis
used by Dart-supported IDEs and code editors.

```bash
dart analyze
```

Running analysis before committing or sharing code helps detect problems
early.

---

## 3. `dart format`

Automatically formats Dart code according to the standard Dart formatting
style.

```bash
dart format .
```

The `.` means that all Dart files in the current directory and its
subdirectories will be formatted.

You can also format a specific file:

```bash
dart format lib/main.dart
```

---
