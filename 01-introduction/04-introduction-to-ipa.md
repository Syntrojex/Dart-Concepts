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
