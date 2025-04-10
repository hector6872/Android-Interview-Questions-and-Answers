## What are Kotlin Coroutines?

Kotlin **Coroutines** are a language feature for writing asynchronous, non-blocking code in a sequential and readable way.

### Why are Coroutines lighter and more efficient than threads?

Coroutines are lighter, more efficient and scalable than threads because they do not require their own thread; instead, they run in existing threads managed by the Kotlin runtime, allowing many coroutines to run concurrently with minimal memory overhead.

## What is _structured concurrency_ in Kotlin and how does it work?

_Structured concurrency_ ensures that coroutines are launched within a specific scope, automatically managing their lifecycle by cancelling them when the scope ends (such as when a function completes or an Activity is destroyed), which helps prevent issues like memory leaks, unfinished tasks, or coroutines running outside of their intended context.