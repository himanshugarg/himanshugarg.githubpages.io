
## Function Declarations
### Scala
{% highlight scala %} 
def sum(a: Int, b: Int): Int = a+b 
{% endhighlight %} 
### Kotlin
{% highlight kotlin %} 
fun sum(a: Int, b: Int): Int = a+b
{% endhighlight %} 

## Passing Functions
### Scala
{% highlight scala %} 
def sumf(f: Int => Int, a: Int, b: Int): Int =
    if (a > b) 0
    else f(a) + sumf(f, a + 1, b)
  
sumf(x => x*x, 1, 5)
{% endhighlight %} 
### Kotlin
{% highlight kotlin %} 
fun sumf(f: (Int) -> Int, a: Int, b: Int): Int =
    if (a > b) 0
    else f(a) + sumf(f, a + 1, b)
        
sumf({ x -> x * x }, 2, 3)
{% endhighlight %} 