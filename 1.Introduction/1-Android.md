# Android — Introduction

## What is Android?

Android is an **Operating System (OS)** designed primarily for mobile
devices. Just as a computer needs an operating system like Windows to
function, mobile hardware — such as the **screen, camera, battery, and
sensors** — needs an operating system to control and coordinate its
resources.

That operating system is **Android**.

> **Android → Operating System for Mobile Devices**

---

## Why Android is Special — Open Source

One of Android's major advantages is its foundation in **open-source
software**. Android is built on the **Android Open Source Project (AOSP)**,
whose source code is publicly available under open-source licenses.

Because of this open foundation, companies such as **Samsung, OPPO, vivo,
and Xiaomi** can build their own customized versions of Android on top of
the AOSP platform.

For example:

- Samsung → **One UI**
- Xiaomi → **HyperOS**
- OPPO → **ColorOS**
- vivo → **OriginOS**

These companies can customize much more than just the visual interface.
They may modify the **user interface, system applications, system
components, platform features, and other parts of the Android experience**.

However, they still build upon the Android platform and its underlying
open-source foundation.

> This is why a Samsung phone and a Xiaomi phone can look and feel very
> different while both supporting Android applications.

---

## Where the Word "Android" Comes From

The word **"Android"** has Greek origins and means **"man-like"** or
**"resembling a human"**:

- **andr-** → man / human
- **-oeidēs** → like / resembling

Historically, the term **android** was used in science fiction and
technology to describe a robot or machine with a human-like appearance.

Google adopted this name for its mobile operating system.

> **Technical definition:** Android is a Linux-kernel-based operating
> system developed primarily by Google and the Android Open Source Project
> (AOSP), designed mainly for mobile devices such as smartphones and
> tablets.

---

## Key Terms to Remember

| Term | Meaning |
|------|---------|
| **Android** | An operating system that manages the hardware and software of a mobile device |
| **Google** | The primary company behind the development of Android |
| **AOSP** | The Android Open Source Project, which provides the open-source foundation of Android |
| **Flutter** | A UI toolkit and framework used to build applications for Android and other platforms using the Dart language |
| **Play Store** | Google's official marketplace for distributing and downloading Android applications |
| **Kernel** | The core part of an operating system that manages hardware resources and provides communication between hardware and software |

---

## Android Versions & API Levels

You've probably heard names like **Android 12**, **Android 13**, or
**Android 14**. These are the public version names of Android.

Behind the scenes, every Android platform release is associated with a
numeric **API Level**. API levels represent the set of platform APIs
available to developers in a particular Android version.

When developers build an app, they specify the minimum Android API level
their app supports. This determines the oldest Android platform on which
the app can run.

> **Example:** If an app supports Android 5.0 and above, its minimum
> supported API level is **API Level 21**.

In modern Android projects, this minimum supported version is commonly
configured through the `minSdk` setting in the project's Gradle
configuration.

| Android Version | API Level |
|-----------------|-----------|
| Android 5.0 (Lollipop) | 21 |
| Android 10 | 29 |
| Android 12 | 31 |
| Android 13 | 33 |
| Android 14 | 34 |

> **Android Version → API Level**
>
> An Android version corresponds to a specific API level. In general,
> newer API levels provide access to newer platform features and APIs.

---

## Quick Recap

> - **Android** = A mobile operating system developed primarily by Google and the Android Open Source Project
> - **AOSP** = The open-source foundation of Android
> - **Open-source foundation** → Allows manufacturers to customize and build their own Android experiences
> - The name **Android** has Greek origins meaning "man-like"
> - Android is based on the **Linux kernel**
> - Each Android platform release is associated with an **API Level**
> - Developers use minimum API levels to define the oldest Android version their app supports
