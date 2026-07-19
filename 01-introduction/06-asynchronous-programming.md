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

## Why Asynchronous Programming Matters in Flutter
Since Flutter apps are UI-driven and constantly need to feel smooth
and responsive, asynchronous programming is a **core requirement**,
not just an optional feature. Any operation that could take unknown or
noticeable time — API calls, file reads/writes, database queries,
image loading — should always be handled asynchronously.

Dart provides built-in tools to make this possible, primarily through:
- **`Future`** — represents a value that will be available at some
  point in the future (used for one-time async operations, like
  fetching data once)
- **`async` / `await`** — keywords used to write asynchronous code in
  a way that looks and reads like normal synchronous code
- **`Stream`** — represents a sequence of asynchronous events over
  time (used when data arrives continuously, like live location
  updates)

> These concepts (`Future`, `async/await`, `Stream`) will be covered
> in detail in dedicated concept files later in this repository.

---
