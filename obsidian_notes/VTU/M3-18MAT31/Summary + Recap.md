#VTU #Math #Recap

### 1. *Laplace Transforms*:
#### Definition and Laplace Transform of Elementary Functions
The Laplace transform of a function \( f(t) \) is defined as:
\[ \mathcal{L}\{f(t)\} = F(s) = \int_0^{\infty} e^{-st} f(t) \, dt \]

#### Laplace Transform of Elementary Functions
1. **Unit Step Function**: \( \mathcal{L}\{u(t)\} = \frac{1}{s} \)
2. **Exponential Function**: \( \mathcal{L}\{e^{at}\} = \frac{1}{s-a} \)
3. **Sine Function**: \( \mathcal{L}\{\sin(bt)\} = \frac{b}{s^2 + b^2} \)
4. **Cosine Function**: \( \mathcal{L}\{\cos(bt)\} = \frac{s}{s^2 + b^2} \)
5. **Polynomial Function**: \( \mathcal{L}\{t^n\} = \frac{n!}{s^{n+1}} \)

#### Laplace Transforms of Periodic Functions and Unit-Step Function
For a periodic function \( f(t) \) with period \( T \):
\[ \mathcal{L}\{f(t)\} = \frac{1}{1 - e^{-sT}} \int_0^T e^{-st} f(t) \, dt \]

For the unit-step function \( u(t-a) \):
\[ \mathcal{L}\{u(t-a)f(t-a)\} = e^{-as}F(s) \]

#### Inverse Laplace Transforms
The inverse Laplace transform is given by:
\[ \mathcal{L}^{-1}\{F(s)\} = f(t) \]

#### Solution of Linear Differential Equations Using Laplace Transforms
To solve \( y'' + ay' + by = f(t) \):
1. Take the Laplace transform of both sides.
2. Use initial conditions.
3. Solve for \( Y(s) \).
4. Find \( y(t) \) by taking the inverse Laplace transform.

#### Example Problem and Solution
**Problem**: Solve \( y'' - 2y' + y = e^t \) with \( y(0) = 0 \), \( y'(0) = 1 \).
1. Laplace Transform: \( (s^2Y(s) - sy(0) - y'(0)) - 2(sY(s) - y(0)) + Y(s) = \frac{1}{s-1} \)
2. Substitute Initial Conditions: \( (s^2Y(s) - 1) - 2sY(s) + Y(s) = \frac{1}{s-1} \)
3. Solve for \( Y(s) \): \( Y(s) = \frac{1}{(s-1)(s-1)} \)
4. Inverse Laplace Transform: \( y(t) = e^t \)

### 2. *Fourier Series*:
#### Periodic Functions and Dirichlet's Condition
A function \( f(t) \) is periodic with period \( T \) if \( f(t+T) = f(t) \).

#### Fourier Series for Periodic Functions with Period 2 and Arbitrary Period
For a function \( f(t) \) with period \( 2L \):
\[ f(t) = a_0 + \sum_{n=1}^{\infty} \left(a_n \cos \frac{n \pi t}{L} + b_n \sin \frac{n \pi t}{L}\right) \]
where
\[ a_0 = \frac{1}{2L} \int_{-L}^L f(t) \, dt \]
\[ a_n = \frac{1}{L} \int_{-L}^L f(t) \cos \frac{n \pi t}{L} \, dt \]
\[ b_n = \frac{1}{L} \int_{-L}^L f(t) \sin \frac{n \pi t}{L} \, dt \]

#### Half-Range Fourier Series
For \( f(t) \) defined only on \( [0, L] \):
\[ f(t) = \frac{a_0}{2} + \sum_{n=1}^{\infty} a_n \cos \frac{n \pi t}{L} \]
where
\[ a_0 = \frac{2}{L} \int_0^L f(t) \, dt \]
\[ a_n = \frac{2}{L} \int_0^L f(t) \cos \frac{n \pi t}{L} \, dt \]

#### Practical Harmonic Analysis with Examples from Engineering
Harmonic analysis decomposes a periodic function into its constituent sine and cosine components. This is useful in engineering for signal processing and vibration analysis.

#### Example Problem and Solution
**Problem**: Find the Fourier series of \( f(t) = t \) on \( [-\pi, \pi] \).
1. Compute coefficients: \( a_0 = 0 \), \( a_n = 0 \), \( b_n = \frac{2(-1)^{n+1}}{n} \).
2. Fourier series: \( f(t) = \sum_{n=1}^{\infty} \frac{2(-1)^{n+1}}{n} \sin(nt) \).

### 3. *Fourier Transforms*:
#### Infinite Fourier Transforms, Fourier Sine, and Cosine Transforms
The Fourier transform of \( f(t) \) is:
\[ \mathcal{F}\{f(t)\} = F(\omega) = \int_{-\infty}^{\infty} f(t) e^{-i\omega t} \, dt \]

#### Fourier Sine and Cosine Transforms
\[ \mathcal{F}_s\{f(t)\} = F_s(\omega) = \int_0^{\infty} f(t) \sin(\omega t) \, dt \]
\[ \mathcal{F}_c\{f(t)\} = F_c(\omega) = \int_0^{\infty} f(t) \cos(\omega t) \, dt \]

#### Inverse Fourier Transforms
\[ \mathcal{F}^{-1}\{F(\omega)\} = f(t) = \frac{1}{2\pi} \int_{-\infty}^{\infty} F(\omega) e^{i\omega t} \, d\omega \]

#### Example Problem and Solution
**Problem**: Find the Fourier transform of \( f(t) = e^{-at}u(t) \).
1. Compute transform: \( F(\omega) = \int_0^{\infty} e^{-at} e^{-i\omega t} \, dt = \frac{1}{a + i\omega} \).

### 4. *Difference Equations and Z-Transforms*:
#### Difference Equations and Basic Definitions
A difference equation relates the difference between successive terms of a sequence.

#### Z-Transforms: Standard Transforms, Damping, and Shifting Rules
The Z-transform of \( f(n) \) is:
\[ \mathcal{Z}\{f(n)\} = F(z) = \sum_{n=0}^{\infty} f(n) z^{-n} \]

#### Initial Value and Final Value Theorems
- **Initial Value Theorem**: \( \lim_{n \to 0} f(n) = \lim_{z \to \infty} (z-1)F(z) \)
- **Final Value Theorem**: \( \lim_{n \to \infty} f(n) = \lim_{z \to 1} (z-1)F(z) \)

#### Example Problem and Solution
**Problem**: Solve \( y[n+1] - 0.5y[n] = u[n] \).
1. Z-transform: \( zY(z) - 0.5Y(z) = \frac{1}{1-z^{-1}} \).
2. Solve: \( Y(z) = \frac{z}{(z-0.5)(z-1)} \).
3. Inverse Z-transform: \( y[n] = 2 \cdot 0.5^n \).

### 5. *Numerical Solutions of Ordinary Differential Equations (ODEs)*:
#### Numerical Solution of First-Order ODEs Using Taylor's Series Method and Modified Euler's Method
- **Taylor's Series Method**: \( y_{n+1} = y_n + hf(x_n, y_n) + \frac{h^2}{2!} f'(x_n, y_n) + \cdots \)
- **Modified Euler's Method**: \( y_{n+1} = y_n + \frac{h}{2} \left( f(x_n, y_n) + f(x_{n+1}, y_{n+1}) \right) \)

#### Fourth-Order Runge-Kutta Method
\[ k_1 = h f(x_n, y_n) \]
\[ k_2 = h f(x_n + \frac{h}{2}, y_n + \frac{k_1}{2}) \]
\[ k_3 = h f(x_n + \frac

{h}{2}, y_n + \frac{k_2}{2}) \]
\[ k_4 = h f(x_n + h, y_n + k_3) \]
\[ y_{n+1} = y_n + \frac{1}{6}(k_1 + 2k_2 + 2k_3 + k_4) \]

#### Milne's Method and Adam-Bashforth Predictor and Corrector Method
- **Milne's Method**: \( y_{n+1} = y_{n-3} + \frac{4h}{3}(2f_{n-2} - f_{n-1} + 2f_n) \)
- **Adam-Bashforth Method**: Predictor and corrector formulas for solving ODEs.

#### Example Problem and Solution
**Problem**: Solve \( y' = xy \) using the fourth-order Runge-Kutta method.
1. Compute \( k_1, k_2, k_3, k_4 \).
2. Update: \( y_{n+1} = y_n + \frac{1}{6}(k_1 + 2k_2 + 2k_3 + k_4) \).

### 6. *Numerical Solution of Second Order ODEs*:
#### Runge-Kutta Method and Milne's Predictor and Corrector Method
- **Runge-Kutta Method**: Similar to the first-order method but applied to second-order equations.
- **Milne's Predictor and Corrector Method**: Used for solving higher-order ODEs with predictor and corrector steps.

#### Example Problem and Solution
**Problem**: Solve \( y'' + y = 0 \) using the Runge-Kutta method.
1. Convert to first-order system.
2. Apply the Runge-Kutta method to the system.

### 7. *Calculus of Variations*:
#### Variation of Function and Functional
A functional is a mapping from a function space to the real numbers.

#### Euler's Equation
\[ \frac{\partial F}{\partial y} - \frac{d}{dx} \left( \frac{\partial F}{\partial y'} \right) = 0 \]

#### Geodesics and Problems Related to Hanging Chains
- **Geodesics**: Shortest path between two points on a surface.
- **Hanging Chains**: Shape of a chain suspended by its ends under gravity (catenary curve).

#### Example Problem and Solution
**Problem**: Find the curve that minimizes \( \int_0^1 (y'^2 + y^2) \, dx \).
1. Euler's Equation: \( 2y'' - 2y = 0 \).
2. Solve: \( y(x) = A \cosh(x) + B \sinh(x) \). 