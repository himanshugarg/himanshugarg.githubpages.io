# Why I am not a Slow (NumPy) Learner 

The first line from [The Basics in the Quickstart tutorial](https://docs.scipy.org/doc/numpy/user/quickstart.html)

> NumPy's main object is the homogeneous multidimensional array. It is a table of elements(usually numbers), all of the same type, indexed by a tuple of positive integers.

Is a multi-dimensional array indeed multi-dimensional? Or is it just a single dimensional array indexed by tuples? Or is there a table? Keep reading, the tutorial, let's.

> In NumPy dimensions are called axes.

Ok, axes must be like the coordinate axes to represent points in a multidimensional space. Good, on the same page!

> For example, the coordinates of a point in 3D space `[1, 2, 1]` has one axis. 

Ouch! Shouldn't that be three axes as that's a point in 3D space. 

> In the example pictured below, the array has 2 axes. The first axis has a length of 2, the second axis has a length of 3.

```python
[[ 1., 0., 0.],
 [ 0., 1., 2.]]
```

Hey, before we get there, did they forget to say what the dots meant? They didn't write `[1.0, 0.0, 0.0]` so there must be a reason behind it. And again what's wrong with using the word dimensions? Something, surely, as we will soon see in the definition of shape.

```python
ndarray.shape
```
> the dimensions of the array. This is a tuple of integers indicating the size of the array in each dimension.

If `ndarray.shape` gives me the array dimensions then I must get 1 for the first and 2 for the second array above, because they are one dimensional and 2 dimensional arrays. Right? No, wrong! The second line says that it is ~~not~~ the dimensions ~~but~~ and its size.

> Arithmetic operators on arrays apply *elementwise*. A new array is created and filled with the result.

Hmm, ok. Let me try to recollect what happens in pure python:-

```python
>>> a = [1, 2, 3] 
>>> b = [4, 5, 6]
>>> c = a+b
>>> a 
[1, 2, 3]
```

Great a new array is created in Python so I know this well. Let's `c`

```python
>>> c
[1, 2, 3, 4, 5, 6]
```

That was neither elementwise nor operation. Some Python unlearning needed here!

> Unlike in many matrix languages, the product operator * operates elementwise in NumPy arrays. The matrix product can be performed using the `dot` function or method:

Oh so there's a method (or function) to the madness and let's call it `def overload(mind)`. The multiplication operator does a dot product and the dot function does matrix multiplication. 

> Some operations, such as `+=` and `*=`, act in place to modify an existing array rather than create a new one.

So this must be how python does **not** do it because numpy is different. Let's check

```python
>>> id(a)
140057043823176
>>> a += [7, 8, 0]
>>> id(a)
140057043823176
```

And I thought, learning this would be quick because I knew Python and this was a **Quickstart**.
