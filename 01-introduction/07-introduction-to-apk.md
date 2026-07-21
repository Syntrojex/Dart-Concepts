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

## APK vs AAB
Originally, APK was the only distribution format for Android apps.
However, Google later introduced a newer, more efficient format:

| Format | Full Name | Use Case |
|--------|-----------|----------|
| **APK** (`.apk`) | Android Package Kit | Can be shared directly with anyone via WhatsApp, Bluetooth, email, etc. — the recipient can install it immediately |
| **AAB** (`.aab`) | Android App Bundle | Required when uploading an app to the **Google Play Store**. Google uses it to generate optimized APKs for each device, resulting in a **smaller overall app size** for end users |

> **Key takeaway:** Use APK for direct sharing/testing, but Play Store
> submissions require AAB.

---

## Generating an APK
Once your Flutter app's code is complete, you generate the installable
APK file using a simple terminal command:

```bash
flutter build apk
```

This command compiles **all your Dart code and Flutter widgets
together** and packages everything into a single `.apk` file, ready
to be installed on an Android device.

---

## How to Run This Command
1. Open **Android Studio**
2. Look at the **bottom-left corner** of the screen — you'll see tabs
   like: `Version Control`, `Run`, `Debug`, `TODO`, and `Terminal`
3. Click on **Terminal**
4. This opens a command-line interface directly at the bottom of your
   IDE, where you can type and run `flutter build apk`

> **Shortcut Key:** `Alt + F12` — opens the terminal instantly without
> needing to click through the tabs manually.

---

## Quick Recap
> - **APK** = Android Package Kit — the installable file format for
>   Android apps, similar to a ZIP file
> - Contains: **DEX files** (compiled code), **Resources**
>   (images/fonts), **AndroidManifest.xml** (permissions/identity),
>   and **Assets** (extra files)
> - **APK** → for direct sharing/sideloading
> - **AAB** → required for Google Play Store uploads (smaller,
>   optimized size)
> - Generate using: `flutter build apk`
> - Quick terminal access shortcut: **Alt + F12**
