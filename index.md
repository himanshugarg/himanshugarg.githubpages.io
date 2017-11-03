
## Function Declarations
### Scala
```scala
def sum(a: Int, b: Int): Int = a+b 
```
### Kotlin
```kotlin
fun sum(a: Int, b: Int): Int = a+b
```

## Passing Functions
### Scala
```scala
def sumf(f: Int => Int, a: Int, b: Int): Int =
    if (a > b) 0
    else f(a) + sumf(f, a + 1, b)
```
```scala
sumf(x => x*x, 1, 5)
```
### Kotlin
```kotlin
fun sumf(f: (Int) -> Int, a: Int, b: Int): Int =
    if (a > b) 0
    else f(a) + sumf(f, a + 1, b)
```
```kotlin
sumf({ x -> x * x }, 2, 3)
```
OR
```kotlin
sumf({ it * it }, 2, 3) // lambda's taking only one parameter as input get a default name
```