# Why I am not a Slow (NumPy) Learner 

I have tried learning NumPy a Number of times. But its inconsistent overloading of operators beats me everytime. See for example [The Basics in the Quickstart tutorial](https://docs.scipy.org/doc/numpy/user/quickstart.html)

> NumPy's main object is the homogeneous multidimensional array. It is a table of elements(usually numbers), all of the same type, indexed by a tuple of positive integers.

Is a multi-dimensional array indeed multi-dimensional? Or is it just a single dimensional array indexed by tuples? Or is it a table?

> In NumPy dimensions are called axes.

Ok, axes must be like the coordinate axes to represent points in a multidimensional space. Or are they?

> For example, the coordinates of a point in 3D space `[1, 2, 1]` has one axis. 

Oops! Shouldn't that be three axes as that's a point in 3D space.

> In the example pictured below, the array has 2 axes. The first axis has a length of 2, the second axis has a length of 3.

```python
[[ 1., 0., 0.],
 [ 0., 1., 2.]]
```

Hey, before we get there, what are the dots? What's wrong with `[1.0, 0.0, 0.0]`. How many man-years were saved by not typing a few zeros. And again what's wrong with using the word dimensions? Something, surely. See the definition of ndarray.shape below.

```python
ndarray.shape
```
> the dimensions of the array. This is a tuple of integers indicating the size of the array in each dimension.

If `ndarray.shape` gives me the array dimensions then I must get 1 for the first and 2 for the second array above, because they are one dimensional and 2 dimensional arrays. Right? No, wrong! The second line says that it is size of the array in each dimension.

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

That was neither elementwise nor operation. Some Python unlearning needed here! But that's not all.

> Unlike in many matrix languages, the product operator * operates elementwise in NumPy arrays. The matrix product can be performed using the `dot` function or method:

Oh so there's a method (or function) to the madness and let's call it ~~def overload(operator)~~ `def overload(mind)`. The multiplication operator does a dot product and the dot function does matrix multiplication. 

> Some operations, such as `+=` and `*=`, act in place to modify an existing array rather than create a new one.

With so many overrides of Python's defaults why only this one had to be mentioned as this is Python's behavior already.

```python
>>> id(a)
140057043823176
>>> a += [7, 8, 0]
>>> id(a)
140057043823176
```

I give up on NumPy until yet another Machine Learning book/tutorial mentions SciPy/NumPy as a prerequisite.
