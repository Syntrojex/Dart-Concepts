 # Dart Documentation

## What is Dart Documentation?

**Dart Documentation** is the collection of official guides, tutorials,
references, and API documentation that help developers learn and use the
Dart programming language.

The main documentation hub is: **[dart.dev](https://dart.dev)**

It is the primary place to learn Dart concepts, explore language features,
read official guides, and find information about Dart tools and packages.

> When you are unsure about a Dart feature, language rule, tool, or best
> practice, official documentation should be one of your first sources to
> check.

---

## Main Sections of dart.dev

The official Dart documentation is organized into several areas, each
serving a different purpose.

| Section | What It Covers |
|---------|----------------|
| **Language Tour** | An example-based introduction to Dart syntax and core language features |
| **Effective Dart** | Official style guidelines and best practices for writing consistent, maintainable code |
| **Library Documentation** | An introduction to the major features of the Dart SDK's core libraries |
| **Dart SDK** | Information about the SDK, its tools, and installation |
| **Learn Dart** | Tutorials and resources for learning Dart |
| **Packages** | Information about Dart's package ecosystem and package management |

A useful way to think about the main documentation is:

```text
dart.dev
│
├── Learn Dart
│   ├── Language Tour
│   ├── Tutorials
│   └── Guides
│
├── Effective Dart
│   └── Style and Best Practices
│
├── Dart SDK
│   └── Tools and Installation
│
├── Library Documentation
│   └── Core Libraries
│
└── Packages
    └── Package Ecosystem
```

---

## Dart API Reference

Alongside the learning documentation, Dart provides a dedicated API
reference:

**[api.dart.dev](https://api.dart.dev)**

The API reference contains detailed documentation for Dart's libraries,
classes, methods, properties, and other APIs.

It covers libraries such as:

- `dart:core`
- `dart:async`
- `dart:collection`
- `dart:convert`
- `dart:math`
- `dart:io`

For example, if you want to know exactly what a class or method does,
you can search for it in the API reference.

### `dart.dev` vs `api.dart.dev`

| Website | Main Purpose |
|---------|--------------|
| **dart.dev** | Learn concepts, language features, tools, and best practices |
| **api.dart.dev** | Look up detailed API documentation for classes, methods, and libraries |

> **Simple rule:**
>
> Use **dart.dev** to learn a concept.
>
> Use **api.dart.dev** to look up the exact API.

---

## Generating Your Own Documentation with `dart doc`

Dart provides the **`dart doc`** command for generating HTML API
documentation from your own Dart code.

This is especially useful when building:

- Dart packages
- Libraries
- Reusable APIs
- Public projects

Before generating documentation for a package, run:

```bash
dart pub get
dart analyze
```

Then generate the documentation:

```bash
dart doc .
```

A complete example:

```bash
cd my_package
dart pub get
dart analyze
dart doc .
```

By default, the generated documentation is placed inside:

```text
doc/api/
```

The generated documentation can then be viewed through a web server.

> `dart doc` generates reference documentation for public Dart APIs from
> your source code and documentation comments.

---

## Writing Documentation Comments

Dart uses documentation comments to describe public classes, methods,
functions, properties, and other APIs.

The most common form is a triple-slash comment:

```dart
/// Calculates the area of a rectangle.
///
/// Takes [width] and [height] as parameters and returns
/// their product.
double calculateArea(double width, double height) {
  return width * height;
}
```

Documentation comments can include:

- Markdown formatting
- Code examples
- Links
- References to other Dart APIs

For example:

```dart
/// Represents a user in the application.
///
/// The [name] parameter stores the user's display name.
class User {
  final String name;

  User(this.name);
}
```

When `dart doc` runs, these comments can become part of the generated
API documentation.

---
