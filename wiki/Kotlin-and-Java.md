## Difference between `var` and `val` in Kotlin

`var` is used for mutable variables, while `val` is used for immutable (read-only) variables.

## What is the `lateinit` modifier?

`lateinit var` allows us to declare a **mutable, non-nullable variable** without initializing it at the point of declaration. It throws an `UninitializedPropertyAccessException` if accessed before being initialized.

### Is `lateinit` thread-safe?

No, `lateinit` is not thread-safe by default. If multiple threads access a `lateinit` variable before it is properly initialized, it can lead to undefined behavior or exceptions. 

## What is `lazy` in Kotlin?

`lazy` is a **property delegate** for **immutable variables** that computes its value only on first access. It is thread-safe by default.

### When to use `lazy`

`lazy` should be used when an immutable variable needs to be initialized only when it is first accessed, improving performance by avoiding unnecessary computation or deferring it.
