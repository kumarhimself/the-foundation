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

### Properties of Definite Integrals
$$\int_a^bf(x)dx=-\int_b^af(x)dx$$
$$\int_a^af(x)dx=0$$
$$\int_a^bcf(x)dx=c\int_a^bf(x)dx$$
$$\int_a^b[f(x) \pm g(x)]dx=\int_a^bf(x)dx \pm \int_a^bg(x)dx$$
$$\int_a^bf(x)dx = \int_a^cf(x)dx + \int_c^bf(x)dx$$
$$\int_a^bcdx=c(b-a)$$
### Net Change Theorem
 - This interpretation of the definite integral states that if $f(x)$ is some quantity and $f'(x)$ is the rate of change of said quantity, then: $$\int_a^bf'(x)dx=f(b)-f(a)$$
 - In other words, computing the integral of the rate of change will output the net change in the quantity
 - This theorem only makes sense if we are integrating a derivative

## Fundamental Theorem of Calculus
### Part One
 - This part tells us how to differentiate definite integrals
 - If $f(x)$ is continuous on $[a, b]$, then: $$g(x)=\int_a^xf(t)dt$$
 - If we differentiate $g(x)$, we get the following: $g'(x)=f(x)$
 - As seen above, the lower limit must be a constant s and the upper limit must be a variable x
 - Important Formulae:
$$\frac{d}{dx}\int_a^{u(x)}f(t)dt = u'(x)f(u(x))$$
$$\frac{d}{dx}\int_{v(x)}^af(t)dt = -\frac{d}{dx}\int_a^{v(x)}f(t)dt=-v'(x)f(v(x))$$
$$\frac{d}{dx}\int_{v(x)}^{u(x)}f(t)dt = -\frac{d}{dx}\left[\int_{v(x)}^af(t)dt+\int_a^{u(x)}f(t)dt\right] = -v'(x)f(v(x)) + u'(x)f(u(x))$$

### Part Two
 - Suppose that $f(x)$ is a continuous function on $[a, b]$ and also suppose that $F(x)$ is the anti-derivative of $f(x)$. Then: $$\int_a^bf(x)=F(x)\vert_a^b=F(b)-F(a)$$
 - When evaluating the integral using this method, don't bother including the constant after integration as it will get cancelled out in the long run

Next Section: [[6-applications-of-integrals]]
