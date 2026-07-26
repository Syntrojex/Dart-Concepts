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

## 6. `dart compile`

Compiles Dart code into another executable format.

For example, you can compile a Dart program into a native executable:

```bash
dart compile exe bin/main.dart -o myapp.exe
```

The generated executable can run directly on the target platform.

Other compilation targets include:

- Native executables
- JavaScript
- WebAssembly

The exact output depends on the compilation command and target you
choose.

> Dart compilation is also an important part of how Dart applications
> are prepared for deployment.

---

## 7. `dart pub get`

Fetches and resolves the dependencies listed in your project's
`pubspec.yaml` file.

```bash
dart pub get
```

For example, if your project has:

```yaml
dependencies:
  http: ^1.0.0
```

Running:

```bash
dart pub get
```

resolves and fetches the required package.

> `pub` is Dart's package management system and is accessed through the
> `dart` command.

---

## 8. `dart pub upgrade`

Updates the project's dependencies to newer versions allowed by the
version constraints in `pubspec.yaml`.

```bash
dart pub upgrade
```

For example, if your project allows compatible newer versions of a
package, this command can update the resolved dependency versions.

---

## 9. `dart pub outdated`

Shows which dependencies have newer versions available.

```bash
dart pub outdated
```

This helps you identify:

- Current dependency versions
- Upgradeable versions
- Latest available versions
- Dependencies that may require major upgrades

---

## 10. `dart test`

Runs the tests in your Dart project.

```bash
dart test
```

Tests help verify that your code behaves as expected and continues to
work correctly as the project grows.

---

## 11. `dart fix`

Shows and applies automated fixes suggested by the Dart analyzer.

To see the available fixes:

```bash
dart fix --dry-run
```

To apply the suggested fixes:

```bash
dart fix --apply
```

These fixes can help with issues such as:

- Deprecated API usage
- Analyzer diagnostics
- Code improvements suggested by Dart

> `dart fix` applies fixes for problems identified by the analyzer. It
> is not a general-purpose code formatter.

---

## 12. `dart info`

Displays diagnostic information about your Dart environment and SDK
installation.

```bash
dart info
```

This can be useful when:

- Troubleshooting Dart setup issues
- Checking environment information
- Reporting problems
- Diagnosing SDK-related issues

---

## 13. `dart pub deps`

Displays the dependency tree of your Dart project.

```bash
dart pub deps
```

This shows:

- Direct dependencies
- Transitive dependencies
- The relationships between packages

For example:

```text
my_project
├── http
│   └── ...
└── path
```

This is useful for understanding which packages your project depends on.

---
