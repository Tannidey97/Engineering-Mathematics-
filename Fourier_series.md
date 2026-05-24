# 💡Fourier Transform
A signal is usually a mixture of many waves with different frequencies, and the Fourier transform separates the signal into its frequency components so we can see which frequencies are present and how strong they are.

# Fourier Transform

## Finite Fourier Sine Transform

The finite Fourier sine transform of $F(x)$, where $0 < x < L$, is defined as:

$$f_s(n) = \int_0^L F(x) \sin\left(\frac{n\pi x}{L}\right) dx$$

where $n$ is an integer.

---

## Inverse Finite Fourier Sine Transform

The function $F(x)$ is called the inverse finite Fourier sine transform of $f_s(n)$ and is given by:

$$F(x) = \frac{2}{L}\sum_{n=1}^{\infty} f_s(n) \sin\left(\frac{n\pi x}{L}\right)$$

---

## Finite Fourier Cosine Transform

The finite Fourier cosine transform of $F(x)$, where $0 < x < L$, is defined as:

$$f_c(n) = \int_0^L F(x) \cos\left(\frac{n\pi x}{L}\right) dx$$

where $n$ is an integer.

---

## Inverse Finite Fourier Cosine Transform

The function $F(x)$ is called the inverse finite Fourier cosine transform of $f_c(n)$ and is given by:

$$F(x) = \frac{1}{L}f_c(0) + \frac{2}{L}\sum_{n=1}^{\infty} f_c(n) \cos\left(\frac{n\pi x}{L}\right)$$
