***A Fourier transform is a method that breaks a signal into its basic frequency parts. 
It tells us which frequencies are inside a signal and how strong each one is.
In simple words, it changes a signal from a “time view” into a “frequency view.”***

**Example intuition:**  
**Suppose a signal is:**  

**f(t) = sin(2t) + 7sin(5t)**  

**The Fourier transform says:** 
**frequency 2 exists with strength 1**  
**frequency 5 exists with strength 7**  

**So it separates mixed waves into individual frequencies.**  
### Some real life examples of Fourier transform  
**When we heard a music, we can hear a combined sound of different frequency.**   
The Fourier transform separates the sound into frequencies like:  
bass → low frequency  
vocals → medium frequency  
sharp instruments → high frequency  


**JPEG images use Fourier-like transforms.**  
Instead of storing every pixel directly, the image is converted into frequency information:
smooth areas → low frequencies
edges/details → high frequencies
Then tiny unnecessary frequencies are removed to reduce file size.
That’s why photos can become very small.  

## Infinite Fourier Transforms ($0 < x < \infty$)

### Infinite Fourier Sine Transform
The infinite Fourier sine transform of a function $F(x)$ where $0 < x < \infty$ is denoted by $f_s(n)$ and is defined as:
$$f_s(n) = \int_{0}^{\infty} F(x) \sin(nx) \, dx$$

### Inverse Infinite Fourier Sine Transform
The function $F(x)$ is called the inverse Fourier sine transform of $f_s(n)$ and is given by:
$$F(x) = \frac{2}{\pi} \int_{0}^{\infty} f_s(n) \sin(nx) \, dn$$

### Infinite Fourier Cosine Transform
The infinite Fourier cosine transform of a function $F(x)$ where $0 < x < \infty$ is denoted by $f_c(n)$ and is defined as:
$$f_c(n) = \int_{0}^{\infty} F(x) \cos(nx) \, dx$$

### Inverse Infinite Fourier Cosine Transform
The function $F(x)$ is called the inverse Fourier cosine transform of $f_c(n)$ and is given by:
$$F(x) = \frac{2}{\pi} \int_{0}^{\infty} f_c(n) \cos(nx) \, dn$$

---

## Finite Fourier Transforms ($0 < x < L$)

### Finite Fourier Sine Transform
The finite Fourier sine transform of $F(x)$ where $0 < x < L$ is defined as ($n$ is an integer):
$$f_s(n) = \int_{0}^{L} F(x) \sin\left(\frac{n\pi x}{L}\right) \, dx$$

### Inverse Finite Fourier Sine Transform
The function $F(x)$ is called the inverse finite Fourier sine transform of $f_s(n)$ and is given by:
$$F(x) = \frac{2}{L} \sum_{n=1}^{\infty} f_s(n) \sin\left(\frac{n\pi x}{L}\right)$$

### Finite Fourier Cosine Transform
The finite Fourier cosine transform of $F(x)$ where $0 < x < L$ is defined as ($n$ is an integer):
$$f_c(n) = \int_{0}^{L} F(x) \cos\left(\frac{n\pi x}{L}\right) \, dx$$

### Inverse Finite Fourier Cosine Transform
The function $F(x)$ is called the inverse finite Fourier cosine transform of $f_c(n)$ and is given by:
$$F(x) = \frac{1}{L} f_c(0) + \frac{2}{L} \sum_{n=1}^{\infty} f_c(n) \cos\left(\frac{n\pi x}{L}\right)$$

---

## General Fourier Transform

*(If neither finite nor infinite is specified, use the infinite/general form).*

$$F(x) = \int_{-\infty}^{\infty} f(t) e^{ixt} \, dt$$

***[Fourier transform works like a projector which actually measures contribution of every possible  frequency
in a signal. Basically it is an analysis of a signal. It analyzes a signal
by frequency view and the strength of the frequency.]***

