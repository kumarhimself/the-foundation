# Introduction to Integrals
#mathematics #calculus-one #integration

## Indefinite Integrals
 - Given a function $F(x)$, the anti-derivative of $F(x)$ is any function $f(x)$ such that: $$f'(x)=F(x)$$
 - If $f(x)$ is any anti-derivative of $F(x)$, then the most general anti-derivative of $F(x)$ is called an indefinite integral, which is denoted as: $$\int F(x)dx = f(x) + c$$
 - In the definition, $\int$ is called the integral symbol, $F(x)$ is the integrand, and c is called the constant of integration
 - The differential is placed after the intergrand to tell us the following:
	1. Which variable to integrate
	2. What to integrate (whatever is in between the integral sign and the differential)

### Properties
$$\int kf(x)dx = k\int f(x)dx$$
$$\int -f(x)dx = -\int f(x)dx$$
$$\int [f(x) \pm g(x)]dx = \int f(x)dx \pm \int g(x)dx$$

## Computing Indefinite Integrals
$$\int x^{n}dx=\frac{x^{n+1}}{n+1} + c, n \ne -1$$
$$\int kdx = kx + c$$
### Integrals of Trigonometric Functions
 - $\int sin(x)dx = -cos(x)+c$
 - $\int cos(x)dx = sin(x)+c$
 - $\int sec^{2}(x)dx = tan(x)+c$
 - $\int sec(x)tan(x)dx = sec(x)+c$
 - $\int csc^{2}(x)dx = -cot(x)+c$
 - $\int csc(x)cot(x)dx = -csc(x)+c$

### Integrals of Inverse Trigonometric Functions
$$\int\frac{1}{x^{2}+1}dx=tan^{-1}(x)$$
$$\int\frac{1}{\sqrt{1-x^{2}}}dx=sin^{-1}(x)$$

### Integrals of Exponential and Logarithmic Functions
 - $\int e^{x}dx = e^{x}+c$
 - $\int a^{x}dx = \frac{a^{x}}{ln(a)} + c$
 - $\int \frac{1}{x}dx=ln(x) + c$

## Substitution Rule
$$\int f(g(x))g'(x)dx = \int f(u)du$$
where $u=g(x)$

## Definite Integrals and the Area Problem
 - How to find area under the curve for non-linear curves?

### Riemann Summations
 - Can estimate area by area by dividing interval into n subintervals, each with a width of: $$\Delta x = \frac{b-a}{n}$$
 - Then, in each subinterval, we can form a rectangle whose height is given by the function value at a specific point in the interval
 - Calculate area of each rectangle and sum it up
	 - Area of each rectangle: $A=\Delta x \cdot f(x_{n})$, where n is the nth subinterval
 - The rectangle height can  take the function value at either the right or left endpoint
	 - One endpoint over estimates the area while the other underestimates the area under the curve
 - Increasing the number of subintervals will make the estimation of the area under the curve more accurate
 - Can use summation (sigma) notation to represent the summation of the rectangles: $$A \approx \sum_{i=1}^{n} f(x_{i})\Delta x$$
 - This is the definition of a Riemann Sum
 - As the number of subintervals (n) increases, the area under the curve will become more accurate
 - In fact, if we let n go out to infinity, we will get the exact area, which can be best represented by the following: $$A \approx \lim_{n \to \infty} \sum_{i=1}^{n} f(x_{i})\Delta x$$
 - $i$ represents the current x-value and the $ith$ rectangle
 - The endpoints of each subinterval are:
	 - $x_{0} = a$
	 - $x_{1} = a + \Delta x$
	 - $x_{2} = a + 2\Delta x$
	 - $x_{i} = a + i\Delta x$
	 - $x_{n - 1} = a + (n - 1)\Delta x$
	 - $x_{n} = a + n\Delta x = b$

### Definition of the Definite Integral
 - Given a function $f(x)$ that is continuous on the interval $[a, b]$ and divided into n subintervals of equal width, $\Delta x$, and from each interval choose a point $x_{i}$, the definite integral of $f(x)$ from a to b is: $$\int_{a}^{b}f(x)dx=\lim_{n \to \infty}\sum_{i=1}^n f(x_{i})\Delta x$$
 - The variables a and b represent the lower and upper limits respectively
	 - Collectively, the variables a and b represents the interval of integration
 - 

Next Section: [[6-applications-of-integrals]]
