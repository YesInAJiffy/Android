# Defining Variables

In Kotlin, you define variables using either the `val` or `var` keyword:

### 1. **Immutable Variable (`val`)**
Use `val` when the variable **cannot be reassigned** after it's initialized (like `final` in Java).

```kotlin
val name: String = "Alice"
```

- Once assigned, `name` cannot be changed.
- Good for constants or values that shouldn't change.

### 2. **Mutable Variable (`var`)**
Use `var` when the variable **can be reassigned**.

```kotlin
var age: Int = 25
age = 26  // This is allowed
```

- Use this when the value is expected to change.

### 3. **Type Inference**
Kotlin can infer the type, so you can omit it if it's obvious:

```kotlin
val city = "New York"  // Inferred as String
var score = 100        // Inferred as Int
```

Would you like to see examples in a specific context, like Android development or data processing?
