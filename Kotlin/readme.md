

# Defining Variables

In Kotlin, you define variables using either the `val` or `var` keyword:

## Playground to be used
https://play.kotlinlang.org/

### 1. **Immutable Variable (`val`)**
Use `val` when the variable **cannot be reassigned** after it's initialized (like `final` in Java).

```kotlin
val name: String = "Alice"
```

- Once assigned, `name` cannot be changed.
- Good for constants or values that shouldn't change.
- Another Example
```kotlin
fun main() {
    val cartTotal = 0
    cartTotal = 20
    println("Total: $cartTotal")
}
```

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

<img width="780" alt="image" src="https://github.com/user-attachments/assets/f2504214-1a03-4ec5-aee1-accbc3c6a44d" />

### In a Program
```kotlin
fun main() {
    val count: Int = 2
    println("You have $count unread messages.")
}
```

### Variable value fetching in string
```kotlin
fun calculateSum(a: Int, b: Int): Int {
    return a + b
}

fun main() {
    val num1 = 10
    val num2 = 20
    val sum = calculateSum(num1, num2)
    println("The sum of $num1 and $num2 is: $sum")
}
```

### Another Example
```kotlin
fun main() {
    val unreadCount = 5
    val readCount = 100
    println("You have ${unreadCount + readCount} total messages in your inbox.")
}
```



# Data Types in Kotlin

Kotlin has a rich set of **data types**, which can be broadly categorized into:

---

### 🔹 **Basic Data Types**

| Type       | Description                     | Example             |
|------------|----------------------------------|---------------------|
| `Int`      | 32-bit integer                   | `val age: Int = 30` |
| `Long`     | 64-bit integer                   | `val big: Long = 123456789L` |
| `Short`    | 16-bit integer                   | `val s: Short = 10` |
| `Byte`     | 8-bit integer                    | `val b: Byte = 1`   |
| `Double`   | 64-bit floating point            | `val pi: Double = 3.14` |
| `Float`    | 32-bit floating point            | `val f: Float = 3.14f` |
| `Boolean`  | `true` or `false`                | `val isActive: Boolean = true` |
| `Char`     | A single character               | `val letter: Char = 'A'` |
| `String`   | A sequence of characters         | `val name: String = "Kotlin"` |

---

### 🔹 **Nullable Types**
Kotlin distinguishes between nullable and non-nullable types:

```kotlin
val name: String = "Alice"       // Non-nullable
val nickname: String? = null     // Nullable
```

Use `?` to declare a variable that can hold `null`.

---

### 🔹 **Arrays and Collections**

- **Array**: `val numbers = arrayOf(1, 2, 3)`
- **List**: `val list = listOf("a", "b", "c")`
- **MutableList**: `val mutableList = mutableListOf(1, 2, 3)`
- **Set**: `val set = setOf(1, 2, 2, 3)` // Unique elements
- **Map**: `val map = mapOf("key" to "value")`

---

### 🔹 **Other Types**

- **Any**: The root of the Kotlin class hierarchy (like `Object` in Java).
- **Unit**: Represents no value (similar to `void` in Java).
- **Nothing**: Represents a value that never exists (used for functions that throw exceptions).

---



