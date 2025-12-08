
# 📘 Kotlin Basics – Day 1

Welcome to **Day 1** of Android Learning with Kotlin.  
This README contains all basic Kotlin concepts required to start Android development.

---

## 🚀 Topics Covered Today

- What is Kotlin?
- Variables (`val` and `var`)
- Data Types
- Strings & Templates
- Functions
- If–Else
- When Expression
- Lists (Mutable & Immutable)
- Loops
- Null Safety

---

## 📌 1. What is Kotlin?

Kotlin is a modern, safe, and clean programming language used for:
- Android app development  
- Backend development  
- Cross-platform apps (Kotlin Multiplatform)

It is officially supported by Google.

---

## 📌 2. Variables in Kotlin

### Immutable (cannot change):

### Mutable (can change):
- var age = 20
- age = 21

### 📌 3. Data Types

Kotlin supports:

- Int

- Double

- Float

- Boolean

- Char

- String

Example:

val count: Int = 10
val pi: Double = 3.14
```kotlin
val name = "Ishan"
```

### 📌 4. Strings & Templates
```
val name = "Ishan"
println("My name is $name")
```

### 📌 5. Functions
- Basic function:
```
fun greet() {
    println("Welcome to Kotlin!")
}
```
- Function with parameters:
```
fun add(a: Int, b: Int): Int {
    return a + b
}
```
### 📌 6. If–Else
```
val age = 18

if (age >= 18) {
    println("Adult")
} else {
    println("Minor")
}
```
### 📌 7. When Expression
```
val day = 2

when (day) {
    1 -> println("Monday")
    2 -> println("Tuesday")
    else -> println("Other day")
}
```
### 📌 8. Lists
- Immutable list:
```
val fruits = listOf("Apple", "Banana", "Mango")
```
- Mutable list:
```
val numbers = mutableListOf(1, 2, 3)
numbers.add(4)
```

### 📌 9. Loops
- For loop:
```
for (i in 1..5) {
    println(i)
}
```

While loop:
var x = 1
while (x <= 5) {
    println(x)
    x++
}

### 📌 10. Null Safety

-Kotlin does not allow null by default.

To allow null:
```
var name: String? = null
println(name)
```
