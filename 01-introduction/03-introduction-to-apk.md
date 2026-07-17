# APK — Android Package Kit

## What is an APK?
**APK (Android Package Kit)** is the file format used to package and
distribute apps for the Android operating system. Think of it as
essentially a **ZIP file** — a compressed container that holds
everything an Android app needs to run.

> When you finish writing your Flutter/Dart code, you need to package
> it into a single installable file so users can install it on their
> phones. That packaged file is called an **APK**.

---

## What's Inside an APK?
Just like a gift box contains multiple different items, an APK file
contains several components bundled together:

| Component | Description |
|-----------|--------------|
| **DEX Files** | Your written code, compiled down into machine-readable bytecode (Dalvik Executable format) that the Android runtime can execute |
| **Resources** | All the images, videos, and fonts used inside your app |
| **AndroidManifest.xml** | The app's **"Identity Card"** — declares what permissions the app needs (e.g., Camera access, Internet access), the app's package name, and other essential metadata |
| **Assets** | Any additional raw files you've added to your app (e.g., JSON files, custom fonts, data files) |

---
