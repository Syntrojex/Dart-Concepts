# iOS — Introduction

## What is iOS?

**iOS (iPhone Operating System)** is Apple's mobile operating system
primarily designed for **iPhone devices**.

Unlike Android, iOS is known for being more tightly controlled by Apple,
with Apple controlling the hardware, operating system, and official
software distribution ecosystem.

> **iOS → Operating System for Apple's iPhone Devices**

> **Note:** Apple's iPad devices use **iPadOS**, a separate operating
> system based on the same broader Apple software platform.

---

## iOS is Closed Source

One of the major differences between iOS and Android is their source
models:

- iOS is a **proprietary, closed-source operating system** whose source
  code is controlled by Apple.
- Unlike Android, other companies cannot freely take iOS, modify it, and
  ship it on their own hardware.
- iOS is officially designed and distributed exclusively for Apple's
  supported devices.

| Feature | Android | iOS |
|---------|---------|-----|
| **Source Model** | Open-source foundation (AOSP) | Proprietary / closed-source |
| **Runs On** | Devices from multiple manufacturers | Apple's supported devices |
| **Primary Developer** | Google and the Android Open Source Project (AOSP) | Apple |
| **Customization** | Manufacturers can extensively customize the platform | Tightly controlled by Apple |

---

## Development Tools

Just as Android has **Android Studio** as its primary official
development environment, Apple provides its dedicated development
environment for Apple-platform development called **Xcode**.

| Platform | Primary Development Tool |
|----------|--------------------------|
| **Android** | Android Studio |
| **iOS** | Xcode |

Xcode provides tools for writing, building, testing, debugging, and
distributing applications for Apple's platforms.

---

## The Biggest Restriction — You Need macOS

One of the most important practical considerations when developing for
iOS is Apple's development environment.

> To build, sign, and officially distribute an iOS application using
> Apple's standard development tools, **macOS is required**.

### Working with Flutter

You can write and develop your Flutter and Dart code on:

- Windows
- macOS
- Linux

However, when you need to build and sign the iOS version of your
application using Apple's official toolchain, you need access to a Mac
running macOS.

This means a developer can:

1. Write most of the shared Flutter/Dart code on Windows or Linux.
2. Transfer or access the project on a Mac.
3. Use Apple's toolchain to build, sign, test, and distribute the iOS
   application.

---

## Quick Recap

> - **iOS** = Apple's proprietary mobile operating system primarily used on iPhone
> - **iPadOS** = Apple's dedicated operating system for iPad
> - **Closed Source / Proprietary** — controlled by Apple
> - Other manufacturers cannot freely ship iOS on their own devices
> - Primary development tool: **Xcode**
> - Building and officially signing iOS apps with Apple's standard toolchain requires **macOS**
> - Flutter/Dart code can be written on Windows, macOS, or Linux
> - Installable file format: **IPA** (iOS application archive/package)
