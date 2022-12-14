# Review of Algebra and Trigonometry
#mathematics #calculus-one

## Functions
### What are Functions?
 - Function - an equation where every input, x, corresponds to exactly one output, y
	 - Examples:
		 - $y = x^{2} + 1$ is a function because no matter what x-value you input, the equation will output one value of y
		 - $y^{2} = x + 1$ is not a function because when you square root both sides of the equation and solve for y, you will have two values of x corresponding to one value of y due to the square root
 - Roots - values of x in which the function is equal to zero
 - Domain - set of all x-values that can be plugged into a function and output a real number
	 - Need to avoid division by zero, square roots of negative numbers, logarithms of zero and negative numbers
 - Range - set of all possible y-values that a function can take

### Function Composition
 - Taking the output of one function and using it as an input to another function
	 - $f(g(x)) = (f \cdot g)(x)$

### Inverse Functions
 - One-to-One Function - a function where no two x-values produces the same y
	 - $f(x_{1}) \neq f(x_{2})$ whenever $x_{1} \neq x_{2}$
	 - A function is one-to-one whenever we plug different x-values into the function and get different y-values
	 - Example: $f(x) = x^2$ is not one-to-one because both $f(-2) = 4$ and $f(2) = 4$
 - Two functions are inverses if $(f \cdot g)(x) = x$ and $(g \cdot f)(x) = x$
	 - Denoted by: $f(x) = g^{-1}(x)$ and $g(x) = f^{-1}(x)$
 - Finding the Inverse of a Function:
	 1. Replace $f(x)$ with y
	 2. Replace every y with x and every x with y simultaneously
	 3. Solve equation for y
	 4. Replace y with $f^{-1}(x)$
	 5. Verify your work by checking that $(f \cdot f^{-1})(x) = x$ and $(f^{-1} \cdot f)(x) = x$
 - The graph of the inverse is always a reflection of the actual function about the line $y = x$

## Trigonometric Functions
 - Remember this table:

| Degrees | Radians | sinx | cosx | tanx |
| ------- | ------- | ---- | ---- | ---- |
| 0       | 0       | 0      | 1     | 0     |
| 30      | $\pi/6$ | $\frac{1}{2}$     | $\frac{\sqrt3}{2}$     | $\frac{1}{\sqrt3}$     |
| 45      | $\pi/4$ | $\frac{\sqrt2}{2}$     | $\frac{\sqrt2}{2}$     | 1     |
| 60      | $\pi/3$ | $\frac{\sqrt3}{2}$     | $\frac{1}{2}$     | $\sqrt3$     |
| 90      | $\pi/2$ | 1     | 0     | Undefined     |
 - You can determine in which quadrant the angle lies by multiplying $0, \frac{\pi}{2}, \pi, \frac{3\pi}{2},$ and $2\pi$ by a number to get the common denominator and determine in which interval the angle lies
	 - Example: Find the quadrant that $\frac{2\pi}{3}$ lies in
		 - Finding the common denominator of $0, \frac{\pi}{2}, \pi, \frac{3\pi}{2},$ and $2\pi$ that corresponds to $\frac{2\pi}{3}$, we get $0, \frac{3\pi}{6}, \frac{6\pi}{6}, \frac{9\pi}{6}, and \frac{12\pi}{6}$. As we can see, the angle is in between $\frac{3\pi}{6}$ and $\frac{6\pi}{6}$ and therefore, $\frac{2\pi}{3}$ lies in the second quadrant.
 - Also remember this acronym:
	 - A: sine, cosine, tangent are positive in the first quadrant
	 - S: only sine is positive in the second quadrant
	 - T: only tangent is positive in the third quadrant
	 - C: only cosine is posititve in the fourth quadrant
 - You can tell which angle has the same value (not including sign) as the one above by looking at the denominator
	 - Evaluate $sin(\frac{2\pi}{3})$ - Since the denominator of the angle is 3, we know that it corresponds to $\frac{\pi}{3}$ from the table, and therefore, we know that the value of the expression is $-\frac{\sqrt{3}}{2}$ (it is also negative because of the ASTC ancronym)

## Summation (Sigma) Notation
 - Let's say we have two integers n and m, with $n < m$ and a list of numbers denoted as: $$a_{n}, a_{n+1}, a_{n+2}, \ldots, a_{m-2}, a_{m-1}, a_{m}$$
 - Adding them up will get the following: $$a_{n} + a_{n+1} + a_{n+2} + \ldots + a_{m-2} + a_{m-1} + a_{m}$$
 - In order to simplify this notation we can write the following: $$\sum_{i=n}^ma_{i} = a_{n} + a_{n+1} + a_{n+2} + \ldots + a_{m-2} + a_{m-1} + a_{m}$$
 - This notation tells us to add up all the $a_{i}$ for all integers starting at n and ending at m
 - $i$ is the initial number and m is the limit of the summation

### Properties
 - If c is a constant, then: $$\sum_{i=i_{0}}ca_{i} = c\sum_{i=i_{0}}a_{i}$$
 - We can break a summation across a sum or difference: $$\sum_{i=i_{0}}^n(a_{i} \pm b_{i}) = \sum_{i=i_{0}}^na_{i} \pm \sum_{i=i_{0}}^nb_{i}$$
 - Note that while we can break up sums and differences, we cannot do the same for products and quotients

### Formulae
 - These formulae are only true if $i=1$
$$\sum_{i=1}^nc=cn$$
$$\sum_{i=i_{0}}^ni = \frac{n(n+1)}{2}$$
$$\sum_{i=i_{0}}^ni^{2} = \frac{n(n+1)(2n+1)}{6}$$
$$\sum_{i=i_{0}}^ni^{3} = \left[\frac{n(n+1)}{2}\right]^2$$



Next Section: [[2-limits-and-continuity]]