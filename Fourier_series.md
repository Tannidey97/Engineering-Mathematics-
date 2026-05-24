‎Fourier Series
A Fourier series is a way to represent a repeating (periodic) function as
a sum of simple sine and cosine waves.
‎[only add the periodic waves]
‎
‎🌊Periodic waves - repeats its phase after a certain time or period.
‎Examples : sine, cosine, AC electricity.

‎## The General Equation of Fourier series :
‎
‎For a function $F(x)$ defined over the interval $[-L, L]$, the Fourier series is:
‎
‎$$F(x) = \frac{a_0}{2} + \sum_{n=1}^{\infty} \left[ a_n \cos\left(\frac{n\pi x}{L}\right) + b_n \sin\left(\frac{n\pi x}{L}\right) \right]$$

# General Fourier Series

The Fourier series allows us to represent a periodic function $F(x)$ (with a period of $2L$) as an infinite sum of sines and cosines.

## The General Equation

For a function $F(x)$ defined over the interval $[-L, L]$, the Fourier series is:

$$F(x) = \frac{a_0}{2} + \sum_{n=1}^{\infty} \left[ a_n \cos\left(\frac{n\pi x}{L}\right) + b_n \sin\left(\frac{n\pi x}{L}\right) \right]$$

---

## The Fourier Coefficients

To solve the equation above, the constants $a_0$, $a_n$, and $b_n$ are calculated using these integrals:

* **DC Component ($a_0$):**
  $$a_0 = \frac{1}{L} \int_{-L}^{L} F(x) dx$$

* **Cosine Coefficients ($a_n$):**
  $$a_n = \frac{1}{L} \int_{-L}^{L} F(x) \cos\left(\frac{n\pi x}{L}\right) dx$$

* **Sine Coefficients ($b_n$):**
  $$b_n = \frac{1}{L} \int_{-L}^{L} F(x) \sin\left(\frac{n\pi x}{L}\right) dx$$

---

## Special Case: Period of $2\pi$

If the function has a period of $2\pi$ (where $L = \pi$) over the interval $[-\pi, \pi]$, the equations simplify to:

$$F(x) = \frac{a_0}{2} + \sum_{n=1}^{\infty} \left[ a_n \cos(nx) + b_n \sin(nx) \right]$$

### Coefficients for $2\pi$:
* $$a_0 = \frac{1}{\pi} \int_{-\pi}^{\pi} F(x) dx$$
* $$a_n = \frac{1}{\pi} \int_{-\pi}^{\pi} F(x) \cos(nx) dx$$
* $$b_n = \frac{1}{\pi} \int_{-\pi}^{\pi} F(x) \sin(nx) dx$$

[We use Fourier series when we need to add different kind of waves which are periodic like repeats after a certain time or period to create a complex periodic signal.
You can say A Fourier series is a mathematical method of combining many periodic sine and cosine waves into one periodic function or signal.]
