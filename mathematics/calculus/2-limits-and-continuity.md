# Limits and Continuity
#mathematics #calculus-one #limits

## Tangent Lines and Rates of Change
### What are Tangent Lines?
 - Tangent Line - line that touches some point on the function $f(x)$
	 - Must be parallel to graph at the point in question, meaning that the slope of the tangent is equal to the slope at the point
 - Secant Line - line that touches two points on the function $f(x)$
 - If we try to find the slope of the tangent line at $P = (a, f(a))$, we can use a second point on the graph, namely $Q = (x, f(x))$, to compute the slope of the tangent line at $x = a$. The equation for performing this calculation is: $$m_{PQ} = \frac{f(x) - f(a)}{x - a}$$
 - Real world application of tangent lines:
	 - The secant line can represent an average rate of change (ARC) while the tangent line can represent an instantaneous rate of change (IRC) at $x = a$

### Change in Notation

^253a0e

 - Instead of using the slope of the tangent equation presented above, we can use another equation that is dependant on how far a point is from the tangent line
 - If we want to move a distance of h from $x = a$, then the new point would be located at $x = a + h$ (h can be positive or negative)
 - Replace x in $f(x)$ with $a + h$ and simplfy: $$m_{PQ} = \frac{f(x) - f(a)}{x - a} = \frac{f(a + h) - f(a)}{h}$$

## Introduction to Limits
 - Using the equation above, as the distance h gets smaller, the slope of the tangent becomes more accurate
	 - This idea is known as taking the limit
 - We say that the limit of $f(x)$ is L as x approaches a and write this as: $$\lim_{x \to a} f(x) = L$$
 - Limits can be separated into left and right-hand limits
 - For left-hand limits, we say: $$\lim_{x \to a^-} f(x) = L$$
	 - Provided we can make $f(x)$ as close to L as we want for all x sufficiently close to a with $x < a$ without letting $x = a$
 - For right-hand limits, we say: $$\lim_{x \to a^+} f(x) = L$$
	 - Provided we can make $f(x)$ as close to L as we want for all x sufficiently close to a with $x > a$ without letting $x = a$
 - The left and right-hand limits must equal to eachother in order for the normal limit to exist: $$\lim_{x \to a^-} f(x) = \lim_{x \to a^+} f(x) = L$$

## Limit Properties
 - Assuming that the following exist: $$\lim_{x \to a} f(x) \,\, \lim_{x \to a} g(x)$$ and that c is any constant, the following are true:
$$
\lim_{x \to a} [cf(x)] = c\lim_{x \to a} f(x)
$$
$$
\lim_{x \to a} [f(x) \, \pm \, g(x)] = \lim_{x \to a} f(x) \, \pm \, \lim_{x \to a} g(x) 
$$
$$
\lim_{x \to a} [f(x) \, \cdot \, g(x)] = \lim_{x \to a} f(x) \, \cdot \, \lim_{x \to a} g(x) 
$$
$$
\lim_{x \to a} \left[\frac{f(x)}{g(x)}\right] = \frac{\lim_{x \to a} f(x)}{\lim_{x \to a} g(x)} 
$$
$$
\lim_{x \to a} [f(x)]^2 = \left[\lim_{x \to a} f(x)\right]^n
$$
$$
\lim_{x \to a} c = c
$$
$$
\lim_{x \to a} x = a
$$
### Some Extra Rules
 - If $p(x)$ is a polynomial, then: $$\lim_{x \to a}p(x) = p(a)$$

## Computing Limits
### Squeeze Theorem
 - If $f(x) \le g(x)$ for all x on $[a, b]$, except possibly at $x = c$, and $a \le c \le b$, then: $$\lim_{x \to c}f(x) \le \lim_{x \to c}g(x)$$
 - Squeeze Theorem - suppose that for all x on $[a, b]$, we have: $$f(x) \le h(x) \le g(x)$$and that: $$\lim_{x \to c}f(x)  = \lim_{x \to c}g(x) = L$$ for some $a \le c \le b$. Then, $$\lim_{x \to c} = L$$
 - Also known as the Sandwich, or the Pinching Theorem

## Infinite Limits
### Definition
 - Infinite Limits are special limits that take on the value of: $$\lim_{x \to a} f(x) = \pm\infty$$
 - The function $f(x)$ will have a vertical asymptote at $x = a$ if either the left-hand, right-hand, or the normal limit equals $\pm \infty$

### Properties of Infinite Limits
 - Given the functions $f(x)$ and $g(x)$, suppose that: $$\lim_{x \to c}f(x) = \infty \,\, \lim_{x \to c}g(x) = L$$Then the following are true:
$$
\lim_{x \to c}[f(x) \pm g(x)] = \infty
$$
$$
\lim_{x \to c}[f(x) \cdot g(x)] = \pm\infty
$$
$$
\lim_{x \to c} \left[\frac{g(x)}{f(x)}\right] = 0
$$
 - Property two depends on the sign of $g(x)$

## Limits at Infinity
### Definitions
 - Limits at Infinity are limits that approaches some value L as x approaches: $$\lim_{x \to \pm\infty} f(x)$$
 - If r is a positive rational number and c is any real number, then: $$\lim_{x \to \pm\infty} \frac{c}{x^r} = 0$$
 - If $p(x)=a_{n}x^{n} + a_{n - 1}x^{n - 1} + \ldots + a_{1}x + a_{0}$ is a polynomial of degree n, then: $$\lim_{x \to \pm\infty} p(x) = \lim_{x \to \pm\infty} [a_{n}x^{n}]$$
 - The function $f(x)$ will have a horizontal asymptote at $y = L$ if the following is true: $$\lim_{x \to \pm\infty}f(x) = L$$

## Continuity
 - A function is said to be continuous at $x = a$ if: $$\lim_{x \to a} f(x) = f(a)$$
 - The function is continuous on the interval $[a, b]$ if it is continuous at each point on the interval
 - If a function is continuous at $x = a$, then the following is also true: $$\lim_{x \to a^+} f(x) = f(a) \ \ \lim_{x \to a^-} f(x) = f(a)$$

### Intermediate Value Theorem (IVT)
 - Suppose that $f(x)$ is continuous on $[a, b]$ and let M be an number between $f(a)$ and $f(b)$. Then there exists a number c such that $a < c < b$ and $f(c) = M$
 - A continuous function will take on all values between $f(a)$ and $f(b)$

Next Section: [[3-introduction-to-derivatives]]