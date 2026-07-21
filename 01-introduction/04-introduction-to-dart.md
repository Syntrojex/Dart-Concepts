# Introduction to Dart

## History of Dart
Dart was unveiled by **Google** in **October 2011** at the GOTO
conference in Aarhus, Denmark. At the time, Google's primary goal was
to create a language that could eventually **replace or compete with
JavaScript** as the standard language for building web applications —
JavaScript had well-known performance and structural limitations that
Google wanted to solve.

For its first few years, Dart didn't gain massive traction — it was
seen as "just another language" trying to challenge JavaScript's
dominance in the browser.

Everything changed between **2015 and 2017**, when Google chose Dart
as the language to power a new UI toolkit called **Flutter**. Flutter
allowed developers to build natively compiled apps for mobile, web,
and desktop from a **single codebase**. This partnership completely
transformed Dart's relevance — it went from a relatively unnoticed
language to one of the fastest-growing languages in mobile app
development.

Today, Dart is maintained by Google and is inseparably linked with
Flutter's success.

---

## Key Facts About Dart

| Fact | Detail |
|------|--------|
| **Year Introduced** | 2011 |
| **Owner** | Google |
| **Original Purpose** | To compete with JavaScript |
| **Turning Point** | Gained massive popularity after Flutter's launch (2015–2017) |
| **Syntax Style** | Uses curly braces `{}` like C++, and every statement ends with a semicolon `;` |
| **Pointers** | Dart has **no pointers** — memory is managed automatically |
| **Compilation** | Supports **AOT (Ahead-of-Time) Compilation**, which makes the final compiled app fast and efficient |

---

## Why No Pointers?
Unlike C or C++, Dart does not expose pointers directly to developers.
This design choice means:
- No manual memory address handling
- Fewer memory-related bugs (like dangling pointers or memory leaks)
- Garbage collection automatically manages memory in the background

This makes Dart significantly safer and easier to learn compared to
lower-level languages.

---

## AOT Compilation — Why It Matters
**AOT (Ahead-of-Time) Compilation** means Dart code is compiled
directly into native machine code **before** the app runs — not while
it's running. This results in:
- Faster app startup times
- Better overall runtime performance
- Smooth production-level performance for released apps

> Dart also supports **JIT (Just-in-Time) Compilation** during
> development, which enables Flutter's famous **Hot Reload** feature —
> instantly seeing code changes without restarting the app.

---

## Features of Dart

1. **Object-Oriented and Strongly Typed**
   Dart is built around classes and objects, and every variable has a
   defined type — either explicitly declared or inferred by the
   compiler. This helps catch errors at compile-time rather than at
   runtime.

2. **Follows OOP (Object-Oriented Programming) Principles**
   Dart fully supports the four pillars of OOP:
   - Encapsulation
   - Inheritance
   - Polymorphism
   - Abstraction

3. **A Mixture of JavaScript, Java, and C#**
   Dart combines ideas from all three languages:
   - **JavaScript** → flexibility, async-friendly design
   - **Java** → strong OOP structure
   - **C#** → clean, modern syntax style

---

## Quick Recap
> - Dart was introduced by **Google in 2011**, originally to compete
>   with JavaScript
> - It became truly powerful after **Flutter's launch (2015–2017)**
> - Has **no pointers**, uses **AOT compilation** for fast performance
> - Is **object-oriented, strongly typed**, and follows OOP principles
> - Combines the best of **JavaScript, Java, and C#**
