# iOS — Introduction

## What is iOS?
**iOS (iPhone Operating System)** is Apple's mobile operating system,
built exclusively for Apple's own hardware — **iPhone and iPad**.
Unlike Android, iOS is known for being significantly **stricter** and
more controlled in how it operates and how apps are developed for it.

> **iOS → Operating System of Apple's Mobile Devices**

---

## iOS is Closed Source
This is the single biggest difference between iOS and Android:

- iOS is **"Closed Source"** — Apple owns and fully controls the source
  code
- Unlike Android (which is Open Source and can be customized by
  manufacturers like Samsung or Xiaomi), **no company can copy, modify,
  or ship iOS** on their own hardware
- iOS **only runs on Apple devices** — you will never see iOS running
  on a Samsung or Xiaomi phone, because Apple doesn't license it out

| Feature | Android | iOS |
|---------|---------|-----|
| **Source Model** | Open Source | Closed Source |
| **Runs On** | Multiple manufacturers (Samsung, Xiaomi, etc.) | Only Apple devices (iPhone, iPad) |
| **Owner** | Google | Apple |
| **Customization** | High (manufacturers modify UI) | Very Limited |

---

## Development Tools
Just as Android has **Android Studio** as its official development
environment, Apple has its own dedicated tool for iOS development
called **Xcode**.

| Platform | Official IDE/Tool |
|----------|---------------------|
| **Android** | Android Studio |
| **iOS** | Xcode |

---

## The Biggest Restriction — You Need a Mac
This is one of the most important practical limitations to understand
when developing for iOS:

> To **build** an iOS app (i.e., compile it into a final installable
> file), you **must use a Mac** (MacBook or iMac). Apple's policy does
> **not allow** building iOS apps directly on Windows.

### ✅ The Workaround
You don't need a Mac for everything — only for the final build step:

- You can **write your entire Flutter/Dart codebase on Windows**
  without any issues
- A **Mac (or MacBook) is only required at the compilation/build
  stage**, when you actually need to package the app into a runnable
  iOS file
- Many developers write code on Windows/Linux throughout development,
  and only switch to a Mac (or use cloud-based Mac services) when it's
  time to build and test on iOS

---
