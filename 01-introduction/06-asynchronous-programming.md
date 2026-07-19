# Asynchronous Programming — Introduction

## What is Asynchronous Programming?
In mobile apps, certain tasks naturally take time to complete, such as:

1. **Downloading data** from the internet
2. **Reading a large file** from a database
3. **Processing an image**

If you write your app using **Synchronous programming**, the app's
entire screen **freezes** while that time-consuming task is running.
The user could tap a button, and absolutely nothing would happen until
the task finishes. This kind of unresponsive freezing is commonly
called **"Jank"** in app development.

**Asynchronous programming** solves this problem — it allows the app
to fetch data or perform time-consuming tasks **in the background**,
while the rest of the app (including the UI) remains fully responsive.
The user can continue scrolling, tapping buttons, and interacting with
the app normally, even while data is still being fetched behind the
scenes.

---
