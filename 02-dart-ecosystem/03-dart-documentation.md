# Dart Documentation

## What is Dart Documentation?

**Dart Documentation** is the collection of official guides, tutorials,
references, and API documentation that help developers learn and use the
Dart programming language.

The main documentation hub is:

**[dart.dev](https://dart.dev)**

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
| **Effective Dart** | Official style guidelines and best practices for writing consistent and maintainable code |
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

## Documentation Comments

Dart supports documentation comments using triple-slash comments:

```dart
/// Calculates the area of a rectangle.
double calculateArea(double width, double height) {
  return width * height;
}
```

Documentation comments can be used to describe:

- Classes
- Functions
- Methods
- Properties
- Parameters
- Other public APIs

They can also support Markdown formatting and references to other Dart
APIs.

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

These comments can be processed by `dart doc` to generate API
documentation.

> Documentation comments are introduced here because they are closely
> connected to Dart's documentation system. Their syntax, formatting,
> and detailed usage will be covered later in the **Basics** section.

---

## Staying Updated — What's New

Dart documentation continues to evolve as the Dart language and SDK
develop.

The official **What's New** page tracks important changes made to the
Dart documentation and related sites:

**[What's New](https://dart.dev/resources/whats-new)**

It can include:

- New documentation pages
- New language features
- Changes to existing guides
- New tools and capabilities
- Documentation improvements

The What's New page is useful for developers who want to stay aware of
how the Dart ecosystem is changing.

> If you are learning Dart, you do not need to follow every update.
> However, checking official updates occasionally can help you discover
> important new features and changes.

---

## Where to Find Dart Packages — `pub.dev`

**[pub.dev](https://pub.dev)** is the official package repository for
Dart packages.

Developers can use it to:

- Search for packages
- Read package documentation
- Check package versions
- View dependencies
- Explore source code
- Add packages to their projects

Example:

```yaml
dependencies:
  http: ^1.0.0
```

After adding a package to `pubspec.yaml`, you can retrieve it using:

```bash
dart pub get
```

For Flutter projects, the equivalent command is:

```bash
flutter pub get
```

Many packages on pub.dev also have automatically generated API
documentation that can be accessed through their documentation pages.

---

## A Practical Documentation Workflow

When working with Dart, a useful documentation workflow is:

```text
Have a question
      ↓
Search dart.dev
      ↓
Learn the concept
      ↓
Check api.dart.dev
      ↓
Verify exact classes and methods
      ↓
Search pub.dev
      ↓
Find packages when needed
```

For example:

```text
"I need to work with JSON"
          ↓
Learn the concept on dart.dev
          ↓
Check dart:convert on api.dart.dev
          ↓
Search pub.dev for additional packages if necessary
```

---

## Quick Recap

> - **dart.dev** → Learn Dart concepts, tools, guides, and best practices
> - **api.dart.dev** → Look up detailed API documentation for Dart libraries
> - **`dart doc`** → Generate API documentation from your own Dart code
> - **Documentation comments (`///`)** → Add documentation to your Dart APIs
> - **What's New** → Track updates to Dart documentation and the ecosystem
> - **pub.dev** → Discover and use Dart packages and their documentation

---

## 📚 Further Learning

Documentation comments were introduced here as part of the Dart
documentation ecosystem.

Their detailed syntax and usage will be covered later in the
**Basics → Comments** section, along with other types of Dart comments.

> 📖 **Next Related Topic:** Comments in the **Basics** section.

---

## The Most Important Habit

You do not need to memorize every Dart class, method, or API.

A good developer knows:

> **What to remember — and where to look up what they don't remember.**

The official documentation is one of the most important tools in the
Dart ecosystem.
