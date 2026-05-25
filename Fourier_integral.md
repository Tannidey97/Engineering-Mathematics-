***A Fourier integral is a mathematical method used to represent a non-periodic function 
as a combination of infinitely many sine and cosine waves having continuously varying 
frequencies.***

**[Basically, fourier integral is used to add or reconstruct waves like Fourier series. But this is different from 
Fourier series. In Fourier series we add those waves that have same frequency or discrete multiple 
of one frequency where in the case of Fourier integral we can add waves without worrying about the frequency.
Any frequency is allowed continuously. So frequencies vary continuously, not just at fixed multiples.]**


**Examples : Sound of a clap, earthquake waves, WiFi, Mobile data, Signal filtering etc.**
**These examples are not periodic.So we can't use Fourier series. We must use Fourier integral there.**

## Fourier Integral Equation (General Form)

This double integral is known as the Fourier integral and holds if $x$ is a point of continuity of $f(x)$:

$$f(x) = \frac{1}{2\pi} \int_{-\infty}^{\infty} f(t) \, dt \int_{-\infty}^{\infty} \cos\big(u(x-t)\big) \, du$$

**Here the part**:
cos\big(u(x-t)\big) 
is just a wave 
And the integral says:
“Add waves of every frequency.”

**another part**
f(t) indicates that,
How strong the wave is at point t.

##The total equation be like:

cosine = one musical tone   
f(t) = volume of that tone  
 Without f(t), every tone would have equal strength.  
 But real signals need different strengths.  
So:  
cosine gives the shape of wave   
 f(t) tells how much of it exists   

**In short, It adds cosine waves of all frequencies u, 
where each point t contributes based on f(t),
and the combined effect is evaluated at the point x.**


---

## Fourier Integral for Symmetric Functions

### 1. For an Even Function
When the function is even, the equation simplifies to:

$$f(x) = \frac{2}{\pi} \int_{0}^{\infty} f(t) \, dt \int_{0}^{\infty} \cos(ut) \cos(ux) \, du$$

### 2. For an Odd Function
When the function is odd, the equation simplifies to:

$$f(x) = \frac{2}{\pi} \int_{0}^{\infty} f(t) \, dt \int_{0}^{\infty} \sin(ut) \sin(ux) \, du$$
