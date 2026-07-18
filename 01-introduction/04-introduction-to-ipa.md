# IPA — iOS App Store Package

## What is an IPA?
**IPA (iOS App Store Package)** is the file format used to package and
distribute apps for Apple's iOS operating system. It is the **direct
equivalent of APK, but for iOS** — just as APK is the installable
package for Android, IPA serves the same purpose for iPhones and iPads.

> **IPA → iOS App Store Package**

---

## What's Inside an IPA?
Similar to an APK, an IPA file is also essentially a compressed
package (technically a ZIP archive with a `.ipa` extension) containing
everything the app needs to run:

| Component | Description |
|-----------|--------------|
| **Payload/** | The main folder inside an IPA containing the actual `.app` bundle — your compiled application |
| **Compiled Binary** | Your Dart/Swift/Objective-C code compiled into machine code that iOS devices can execute |
| **Resources** | Images, fonts, videos, and other media assets used in the app |
| **Info.plist** | iOS's equivalent of Android's `AndroidManifest.xml` — this file acts as the app's **"Identity Card"**, storing metadata like app name, permissions, version, and configuration details |
| **Assets.car** | A compiled asset catalog containing app icons, launch images, and other visual resources |

---

## Generating an IPA
Just like Android apps are built using `flutter build apk`, iOS apps
are built using a similar command:

```bash
flutter build ipa
```

> ⚠️ **Important:** Unlike APK generation, building an IPA **requires
> a Mac** (MacBook or iMac) because Apple's build tools (Xcode) only
> run on macOS. You **cannot** generate an IPA file directly on
> Windows or Linux.

### The Workaround (Same as iOS Development in General)
- You can write your entire Flutter/Dart codebase on **Windows or
  Linux** without any problem
- A **Mac is only required at the final build stage**, when compiling
  the code into an actual `.ipa` file
- Developers without a Mac often use cloud-based Mac services (like
  **Codemagic** or **MacinCloud**) to build their IPA remotely

---
