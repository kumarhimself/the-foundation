# Introduction to Derivatives 
#mathematics #calculus-one #differentiation

## Definition of a Derivative
 - The derivative of $f(x)$ with respect to x is the function $f'(x)$ and is defined as: $$f'(x)=\lim_{h \to 0} \frac{f(x + h) - f(x)}{h}$$
 - A function is called differentiable at $ x = a$ if $f'(a)$ exists and $f(x)$ is called differentiable on an interval if the derivative exists for each point in that interval
	 - If $f(x)$ if differentiable at $x = a$, then the function is also continuous
		 - This theorem does not work in reverse!

## Differentiation Properties
 - If $f(x)$ and $g(x)$ are functions and c is some constant, then:
	1. $[f(x) \pm g(x)]' = f'(x) \pm g'(x)$
	2. $(c \, \cdot \, f(x))' = c \, \cdot \, f'(x)$
	3. $(c)' = 0$
	4. $(x^{n})' = nx^{n - 1}$
	5. $(f \, \cdot \, g)' = f'g + fg'$
	6. $\left(\frac{f}{g}\right)' = \frac{f'g - fg'}{g^{2}}$

 ## Derivatives of Trigonometric Functions
 ### Important Limits
$$\lim_{\theta \to 0}\frac{sin(\theta)}{\theta} = 1$$
$$\lim_{\theta \to 0}\frac{cos(\theta) - 1}{\theta} = 0$$

### Derivatives of Trigonometric Functions
1. $[sin(x)]' = cos(x)$
2. $[cos(x)]'=-sin(x)$
3. $[tan(x)]'=sec^{2}(x)$
4. $[csc(x)]'=-csc(x)cot(x)$
5. $[sec(x)]'=sec(x)tan(x)$
6. $[cot(x)]'=-csc^{2}(x)$

### Derivatives of Inverse Trigonometric Functions
$$[sin^{-1}(x)]'=\frac{1}{\sqrt{1-x^{2}}}$$
$$[cos^{-1}(x)]'=-\frac{1}{\sqrt{1-x^{2}}}$$
$$[tan^{-1}(x)]'=\frac{1}{1+x^{2}}$$
$$[csc^{-1}(x)]'=-\frac{1}{|x|\sqrt{x^{2}+1}}$$
$$[sec^{-1}(x)]'=\frac{1}{|x|\sqrt{x^{2}+1}}$$
$$[cot^{-1}(x)]'=-\frac{1}{1+x^{2}}$$

## Derivatives of Exponential and Logarithmic Functions
### Formulae
1. $(e^{x})'=e^{x}$
2. $(ln(x))'=\frac{1}{x}$
3. $(a^{x})'=a^{x}ln(a)$
4. $(\log_{a}x)'=\frac{1}{xln(a)}$

## Chain Rule
 - Suppose that we have two functions, $f(x)$ and $g(x)$ and they are both differentiable. If we define $F(x)=(f \cdot g)(x)$, then the derivative of $F(x)$ is: $$F'(x) = f'(g(x)) \cdot g'(x)$$

Next Section: [[4-applications-of-derivatives]]