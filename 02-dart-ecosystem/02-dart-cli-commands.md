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

## 4. `dart doc`

Generates HTML API documentation from documentation comments in your
Dart code.

```bash
dart doc .
```

Documentation comments are written using `///`.

Example:

```dart
/// Calculates the area of a rectangle.
double calculateArea(double width, double height) {
  return width * height;
}
```

The complete concept of Dart documentation and documentation comments is
covered in the **Dart Documentation** section.

---

## 5. `dart create`

Creates a new Dart project using one of Dart's built-in project
templates.

```bash
dart create my_project
```

This creates a new project directory with the required project files.

Dependencies are fetched automatically unless you use:

```bash
dart create --no-pub my_project
```

> Flutter has a similar command for creating Flutter projects:
> `flutter create`.

---
