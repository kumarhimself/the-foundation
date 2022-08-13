# Applications of Derivatives
#mathematics #calculus-one #differentiation

## Rates of Change
 - As mentioned before, the derivative of a function $f(x)$ represents the rate of change of a quantity at some x-value
 - If the derivative is positive on an interval, then the function is increasing on that interval
 - If the derivative is negative on an interva, then the function is decreasing on that interval
 - In order to find where the function $f(x)$ is increasing and decreasing, follow the steps below:
	1. Find all roots of $f(x)$
	2. Take the derivative of $f(x)$
	3. Pick a x-value between each of the roots
	4. Insert each of the x-value into $f'(x)$
	5. If the derivative returns a positive value, $f(x)$ is increasing on that interval, otherwise,  $f(x)$ is decreasing on that interval

## Critical Points and Extrema
### Critical Points
 - We say that $x=c$ is a critical point of the function $f(x)$ if $f(c)$ exists, and that $f'(c)$ either equals to zero or doesn't exist
	 - Distinct from the roots of a function

### Extrema
 - Types of Extrema:
	 - Global Maxima - the point at which the function is at its highest
	 - Global Minima - the point at which the function is at its highest
	 - Local Maxima - point at which the interval is at its highest
	 - Local Minima - point at which the interval is at its highest
 - Extrema occur at the critical points of a function

### Extreme Value Theorem
 - Suppose that $f(x)$ is continuous on the interval $[a, b]$. Then, there are two numbers $a \le c$ and $d \le b$. Because of this, $f(c)$ is an absolute maximum, and $f(d)$ is an absolute minimum for the function

### Finding Absolute Extrema
 - Assuming that a function $f(x)$ is continuous on the interval $[a, b]$, follow these steps:
 1. Find all critical points of $f(x)$ that are in the $[a, b]$
 2. Evaluate $f(x)$ at the critical and end points
 3. Identify the absolute extrema

## Shape of a Graph
 - Functions are made up of intervals that are concave up or down
	 - Concave Up - interval where all of the tangents to the curve are below the graph of $f(x)$
	 - Concave Down - interval where all the tangents to the curve are above the graph of $f(x)$
 - Inflection Point - point where the concavity changes
 - Given the function $f(x)$, then:
	 - If $f''(x) > 0$ for all x in some interval, then $f(x)$ is concave up on that interval
	 - If $f''(x) < 0$ for all x in some interval, then $f(x)$ is concave down on that interval

### Second Derivative Test
 - Suppose that $x = c$ is a critical point of $f(x)$ and that $f''(x)$ is continuous in a region around $x = c$. Then:
	 - If $f''(x) < 0$, then $x = c$ is a relative maximum
	 - If $f''(x) > 0$, then $x = c$ is a relative minimum
	 - If $f''(x) = 0$, then $x = c$ can be either a relative minimum or maximum, or neither

## Mean Value Theorem
### Rolle's Theorem
 - Suppose $f(x)$ is a function that satisfies the following:
	 - $f(x)$ is continuous on the closed interval $[a, b]$
	 - $f(x)$ is differentiable on the open interval $(a, b)$
	 - $f(a) = f(b)$
 - Then, there is a number c such that $a < c < b$ and $f'(c) = 0$

### Mean Value Theorem
 - Suppose $f(x)$ is a function that satisfies the following:
	 -  $f(x)$ is continuous on the closed interval $[a, b]$
	 - $f(x)$ is differentiable on the open interval $(a, b)$
 - Then, there is a number c such that $a < c < b$ and: $$f'(c) = \frac{f(b)-f(a)}{b-a}$$

## L'Hospital's Rule and Indeterminate Forms
 - Suppose that we have one of the following cases: $$\lim_{x \to a}\frac{f(x)}{g(x)}=\frac{0}{0} \ or \ \lim_{x \to a}\frac{f(x)}{g(x)}=\frac{\pm\infty}{\pm\infty}$$
	L'Hospital's rule dictates that the following can be applied to solve these problems: $$\lim_{x \to a}\frac{f(x)}{g(x)}=\lim_{x \to a}\frac{f'(x)}{g'(x)}$$

## Differentials
 - Given a function $y = f(x)$, we call $dy$ and $dx$ differentials and the relationship between them is given by: $$dy = f'(x)dx$$

## Linear Approximation and Newton's Method
 - Linear Approximation and Newton's Method are two ways of approximating equations at specific points

### Linear Approximation
 - Linear Approximation - approximation of a general function using a linear function
 - Linear function is defined as: $$f(x) = f(a) + f'(a)(x-a)$$
	Where a is a point close to x that is easier to evaluate.
 - Steps:
	1. Identify the general function
	2. Find a number (represented as point a) that is close to x and can easily be evaulated in the function
	3. Take the derivative of the function
	4. Plug in the values and find the approximation

### Newton's Method
 - Newton's Method - method of finding the roots of a function
 - Steps:
	1. Pick a value of x and evaluate the function at that value of x
	2. If the function evaluated at x isn't an approximation of zero, then use the equation below to find the root: $$x_{n+1}=x_{n}-\frac{f(x_{n})}{f'(x_{n})}$$
	3. Evaluate the function at $x_{n+1}$
	4. Keep on following steps 1-3 until you find a value of x in which the function is an approximation of zero

Next Section: [[5-introduction-to-integrals]]