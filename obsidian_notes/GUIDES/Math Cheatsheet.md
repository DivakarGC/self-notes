#Cheatsheet #Math 

---

# Math Cheatsheet for Engineering

## Fundamental Algebra

### Variables and Expressions
$$
\begin{aligned}
&a + b = c \\
&a - b = d \\
&a \cdot b = e \\
&\frac{a}{b} = f \quad (\text{where } b \neq 0)
\end{aligned}
$$

### Equations and Inequalities
$$
\begin{aligned}
&3x + 5 = 11 \\
&2y - 7 < 5y + 3
\end{aligned}
$$

### Functions
$$
\begin{aligned}
&f(x) = ax + b \\
&g(x) = x^2 + 3x - 2
\end{aligned}
$$

### Exponents and Logarithms
$$
\begin{aligned}
&a^m \cdot a^n = a^{m+n} \\
&\frac{a^m}{a^n} = a^{m-n} \\
&\log_b(xy) = \log_b(x) + \log_b(y)
\end{aligned}
$$

### Quadratic Equations
$$
\begin{aligned}
&ax^2 + bx + c = 0 \\
&x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
\end{aligned}
$$

### Applications
- **Circuit Analysis**: Ohm's Law, \(V = IR\)
- **Signal Processing**: Amplitude modulation

### Examples

#### Example 1: Solving Linear Equations
- **Problem:** Solve for \(x\) in \(2x - 5 = 7\)
- **Solution:**
  $$
  \begin{aligned}
  &2x - 5 = 7 \\
  &2x = 7 + 5 \quad (\text{add 5 to both sides}) \\
  &2x = 12 \\
  &x = \frac{12}{2} \quad (\text{divide both sides by 2}) \\
  &x = 6
  \end{aligned}
  $$

#### Example 2: Solving Quadratic Equations
- **Problem:** Solve for \(x\) in \(x^2 - 4x + 4 = 0\)
- **Solution:**
  $$
  \begin{aligned}
  &x^2 - 4x + 4 = 0 \\
  & (x-2)^2 = 0 \quad (\text{factoring}) \\
  & x - 2 = 0 \\
  & x = 2
  \end{aligned}
  $$

#### Example 3: Solving Inequalities
- **Problem:** Solve \(2y - 7 < 5y + 3\)
- **Solution:**
  $$
  \begin{aligned}
  &2y - 7 < 5y + 3 \\
  &-7 - 3 < 5y - 2y \quad (\text{subtract 5y and 3 from both sides}) \\
  &-10 < 3y \\
  &\frac{-10}{3} < y \quad (\text{divide both sides by 3}) \\
  &y > -\frac{10}{3}
  \end{aligned}
  $$

#### Example 4: Circuit Analysis
- **Problem:** Find the current \(I\) in a circuit where \(V = 12V\) and \(R = 3\Omega\)
- **Solution:**
  $$
  \begin{aligned}
  &V = IR \\
  &12 = I \cdot 3 \\
  &I = \frac{12}{3} \\
  &I = 4A
  \end{aligned}
  $$

#### Example 5: Signal Processing
- **Problem:** Find the modulated signal for \(A_m = 2\), \(A_c = 5\), \(\omega_c = 1000\) rad/s, and \(m(t) = \cos(500t)\)
- **Solution:**
  $$
  \begin{aligned}
  &s(t) = A_c[1 + A_m m(t)]\cos(\omega_c t) \\
  &s(t) = 5[1 + 2\cos(500t)]\cos(1000t)
  \end{aligned}
  $$

---

## Pre-Linear Algebra

### Matrices & Vectors
$$
\mathbf{A} = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}, \quad \mathbf{B} = \begin{pmatrix} 0 & -1 \\ 2 & 5 \end{pmatrix}
$$

### Systems of Linear Equations
$$
\begin{aligned}
&2x + 3y = 8 \\
&4x - y = 2
\end{aligned}
$$

### Determinants and Inverses
$$
\text{det}(\mathbf{A}), \quad \mathbf{A}^{-1}
$$

### Applications
- **Control Systems**: State-space representation in autopilot systems

### Examples

#### Example 1: Solving a System of Linear Equations (Substitution)
- **Problem:** Solve for \(x\) and \(y\) in:
  $$
  \begin{cases}
  2x + 3y = 8 \\
  4x - y = 2
  \end{cases}
  $$
- **Solution:**
  $$
  \begin{aligned}
  &\text{From } 2x + 3y = 8: \\
  & 2x = 8 - 3y \\
  & x = 4 - \frac{3y}{2} \quad (\text{divide by 2}) \\
  \\
  &\text{Substitute } x = 4 - \frac{3y}{2} \text{ into } 4x - y = 2: \\
  & 4(4 - \frac{3y}{2}) - y = 2 \\
  & 16 - 6y - y = 2 \\
  & -7y = -14 \\
  & y = 2 \\
  \\
  &\text{Substitute } y = 2 \text{ back into } x = 4 - \frac{3y}{2}: \\
  & x = 4 - \frac{3 \cdot 2}{2} \\
  & x = 4 - 3 \\
  & x = 1
  \end{aligned}
  $$
  Therefore, \(x = 1\) and \(y = 2\).

#### Example 2: Finding the Determinant of a Matrix
- **Problem:** Find the determinant of \(\mathbf{A} = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}\)
- **Solution:**
  $$
  \begin{aligned}
  &\text{det}(\mathbf{A}) = \begin{vmatrix} 1 & 2 \\ 3 & 4 \end{vmatrix} \\
  & = (1 \cdot 4) - (2 \cdot 3) \\
  & = 4 - 6 \\
  & = -2
  \end{aligned}
  $$

#### Example 3: Finding the Inverse of a Matrix
- **Problem:** Find the inverse of \(\mathbf{A} = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}\)
- **Solution:**
  $$
  \begin{aligned}
  & \mathbf{A}^{-1} = \frac{1}{\text{det}(\mathbf{A})} \begin{pmatrix} d & -b \\ -c & a \end{pmatrix} \quad \text{where } \mathbf{A} = \begin{pmatrix} a & b \\ c & d \end{pmatrix} \\
  & = \frac{1}{-2} \begin{pmatrix} 4 & -2 \\ -3 & 1 \end{pmatrix} \\
  & = \begin{pmatrix} -2 & 1 \\ 1.5 & -0.5 \end{pmatrix}
  \end{aligned}
  $$

#### Example 4: Control Systems
- **Problem:** Represent the system \(x' = 2x + 3y, y' = 4x - y\) in state-space form.
- **Solution:**
  $$
  \begin{aligned}
  &\mathbf{x'} = \mathbf{Ax} \\
  &\mathbf{x'} = \begin{pmatrix} x' \\ y' \end{pmatrix}, \quad \mathbf{x} = \begin{pmatrix} x \\ y \end{pmatrix} \\
  &\mathbf{A} = \begin{pmatrix} 2 & 3 \\ 4 & -1 \end{pmatrix} \\
  &\

text{State-space form:} \quad \begin{pmatrix} x' \\ y' \end{pmatrix} = \begin{pmatrix} 2 & 3 \\ 4 & -1 \end{pmatrix} \begin{pmatrix} x \\ y \end{pmatrix}
  \end{aligned}
  $$

---

## Trigonometry Fundamentals

### Basic Trigonometric Functions
$$
\sin(\theta), \cos(\theta), \tan(\theta)
$$

### Pythagorean Identity
$$
\sin^2(\theta) + \cos^2(\theta) = 1
$$

### Trigonometric Identities
$$
\begin{aligned}
&\sin(2\theta) = 2\sin(\theta)\cos(\theta) \\
&\cos(2\theta) = \cos^2(\theta) - \sin^2(\theta)
\end{aligned}
$$

### Applications
- **Antenna Design**: Calculating radiation patterns using trigonometric functions

### Examples

#### Example 1: Basic Trigonometric Values
- **Problem:** Find \(\sin(30^\circ)\)
- **Solution:**
  $$
  \sin(30^\circ) = \frac{1}{2}
  $$

#### Example 2: Using Pythagorean Identity
- **Problem:** If \(\sin(\theta) = \frac{3}{5}\), find \(\cos(\theta)\)
- **Solution:**
  $$
  \begin{aligned}
  &\sin^2(\theta) + \cos^2(\theta) = 1 \\
  &\left(\frac{3}{5}\right)^2 + \cos^2(\theta) = 1 \\
  &\frac{9}{25} + \cos^2(\theta) = 1 \\
  &\cos^2(\theta) = 1 - \frac{9}{25} \\
  &\cos^2(\theta) = \frac{25}{25} - \frac{9}{25} \\
  &\cos^2(\theta) = \frac{16}{25} \\
  &\cos(\theta) = \pm \frac{4}{5}
  \end{aligned}
  $$

#### Example 3: Applying Trigonometric Identities
- **Problem:** Find \(\sin(2\theta)\) if \(\sin(\theta) = \frac{1}{3}\) and \(\cos(\theta) = \frac{2\sqrt{2}}{3}\)
- **Solution:**
  $$
  \begin{aligned}
  &\sin(2\theta) = 2\sin(\theta)\cos(\theta) \\
  & = 2 \left(\frac{1}{3}\right) \left(\frac{2\sqrt{2}}{3}\right) \\
  & = \frac{2 \cdot 1 \cdot 2\sqrt{2}}{3 \cdot 3} \\
  & = \frac{4\sqrt{2}}{9}
  \end{aligned}
  $$

#### Example 4: Antenna Design
- **Problem:** Calculate the radiation pattern of an antenna given \(\theta = 45^\circ\)
- **Solution:**
  $$
  \begin{aligned}
  &\text{Radiation pattern formula:} \quad E(\theta) = E_0 \cos(\theta) \\
  &E(45^\circ) = E_0 \cos(45^\circ) \\
  &E(45^\circ) = E_0 \left(\frac{\sqrt{2}}{2}\right) \\
  &\text{For } E_0 = 1, \quad E(45^\circ) = \frac{\sqrt{2}}{2}
  \end{aligned}
  $$

---

## Linear Algebra

### Vector Operations
$$
\mathbf{u} = \begin{pmatrix} u_1 \\ u_2 \\ u_3 \end{pmatrix}, \quad \mathbf{v} = \begin{pmatrix} v_1 \\ v_2 \\ v_3 \end{pmatrix}
$$

### Matrix Operations
$$
\mathbf{A} = \begin{pmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{pmatrix}, \quad \mathbf{B} = \begin{pmatrix} b_{11} & b_{12} \\ b_{21} & b_{22} \end{pmatrix}
$$

### Eigenvalues and Eigenvectors
$$
\mathbf{A}\mathbf{x} = \lambda \mathbf{x}
$$

### Applications
- **Robotics**: Kinematic transformations using homogeneous matrices

### Examples

#### Example 1: Vector Addition
- **Problem:** Find \(\mathbf{u} + \mathbf{v}\) where \(\mathbf{u} = \begin{pmatrix} 1 \\ 2 \\ 3 \end{pmatrix}\) and \(\mathbf{v} = \begin{pmatrix} 4 \\ 5 \\ 6 \end{pmatrix}\)
- **Solution:**
  $$
  \begin{aligned}
  &\mathbf{u} + \mathbf{v} = \begin{pmatrix} 1 \\ 2 \\ 3 \end{pmatrix} + \begin{pmatrix} 4 \\ 5 \\ 6 \end{pmatrix} \\
  & = \begin{pmatrix} 1 + 4 \\ 2 + 5 \\ 3 + 6 \end{pmatrix} \\
  & = \begin{pmatrix} 5 \\ 7 \\ 9 \end{pmatrix}
  \end{aligned}
  $$

#### Example 2: Matrix Multiplication
- **Problem:** Find \(\mathbf{A}\mathbf{B}\) where \(\mathbf{A} = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}\) and \(\mathbf{B} = \begin{pmatrix} 0 & -1 \\ 2 & 5 \end{pmatrix}\)
- **Solution:**
  $$
  \begin{aligned}
  &\mathbf{A}\mathbf{B} = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix} \begin{pmatrix} 0 & -1 \\ 2 & 5 \end{pmatrix} \\
  & = \begin{pmatrix} 1\cdot 0 + 2\cdot 2 & 1\cdot(-1) + 2\cdot 5 \\ 3\cdot 0 + 4\cdot 2 & 3\cdot(-1) + 4\cdot 5 \end{pmatrix} \\
  & = \begin{pmatrix} 4 & 9 \\ 8 & 17 \end{pmatrix}
  \end{aligned}
  $$

#### Example 3: Finding Eigenvalues
- **Problem:** Find the eigenvalues of \(\mathbf{A} = \begin{pmatrix} 1 & 2 \\ 2 & 1 \end{pmatrix}\)
- **Solution:**
  $$
  \begin{aligned}
  &\text{Characteristic equation:} \\
  &\det(\mathbf{A} - \lambda \mathbf{I}) = 0 \\
  &\begin{vmatrix} 1 - \lambda & 2 \\ 2 & 1 - \lambda \end{vmatrix} = 0 \\
  & (1 - \lambda)(1 - \lambda) - 4 = 0 \\
  & (\lambda - 3)(\lambda + 1) = 0 \\
  & \lambda = 3 \quad \text{or} \quad \lambda = -1
  \end{aligned}
  $$

#### Example 4: Robotics
- **Problem:** Find the homogeneous transformation matrix for a translation of \(x = 2\), \(y = 3\), and \(z = 4\)
- **Solution:**
  $$
  \begin{aligned}
  &\text{Homogeneous transformation matrix:} \\
  &\mathbf{T} = \begin{pmatrix}
  1 & 0 & 0 & x \\
  0 & 1 & 0 & y \\
  0 & 0 & 1 & z \\
  0 & 0 & 0 & 1
  \end{pmatrix} \\
  &\mathbf{T} = \begin{pmatrix}
  1 & 0 & 0 & 2 \\
  0 & 1 & 0 & 3 \\
  0 & 0 & 1 & 4 \\
  0 & 0 & 0 & 1
  \end{pmatrix}
  \end{aligned}
  $$

---

## Pre-Calculus

### Polynomial Functions
$$
P(x) = a_n x^n + a_{n-1} x^{n-1} + \ldots + a_1 x + a_0
$$

### Rational Functions
$$
R(x)

 = \frac{P(x)}{Q(x)} \quad (Q(x) \neq 0)
$$

### Exponential and Logarithmic Functions
$$
\begin{aligned}
&y = a^x \\
&y = \log_b(x)
\end{aligned}
$$

### Applications
- **Signal Processing**: Exponential growth in signal amplification

### Examples

#### Example 1: Polynomial Evaluation
- **Problem:** Evaluate \(P(x) = 2x^3 - 3x^2 + x - 5\) at \(x = 2\)
- **Solution:**
  $$
  \begin{aligned}
  &P(2) = 2(2^3) - 3(2^2) + 2 - 5 \\
  & = 2(8) - 3(4) + 2 - 5 \\
  & = 16 - 12 + 2 - 5 \\
  & = 1
  \end{aligned}
  $$

#### Example 2: Simplifying Rational Functions
- **Problem:** Simplify \(R(x) = \frac{x^2 - 1}{x + 1}\)
- **Solution:**
  $$
  \begin{aligned}
  &R(x) = \frac{(x + 1)(x - 1)}{x + 1} \\
  & = x - 1 \quad (\text{for } x \neq -1)
  \end{aligned}
  $$

#### Example 3: Evaluating Logarithmic Functions
- **Problem:** Evaluate \(\log_2(8)\)
- **Solution:**
  $$
  \begin{aligned}
  &\log_2(8) = x \\
  &2^x = 8 \\
  &2^x = 2^3 \\
  &x = 3
  \end{aligned}
  $$

#### Example 4: Signal Processing
- **Problem:** Calculate the amplified signal for an exponential growth model with initial amplitude \(A_0 = 2\) and growth rate \(k = 0.5\) over time \(t = 4\)
- **Solution:**
  $$
  \begin{aligned}
  &A(t) = A_0 e^{kt} \\
  &A(4) = 2 e^{0.5 \cdot 4} \\
  &A(4) = 2 e^2 \\
  &A(4) \approx 2 \cdot 7.389 \\
  &A(4) \approx 14.778
  \end{aligned}
  $$

---

## Calculus

### Limits and Continuity
$$
\lim_{x \to a} f(x)
$$

### Differentiation
$$
f'(x) = \frac{df(x)}{dx}
$$

### Integration
$$
\int f(x) \, dx
$$

### Applications
- **Control Systems**: PID controller tuning using differentiation and integration

### Examples

#### Example 1: Finding Limits
- **Problem:** Find \(\lim_{x \to 2} (x^2 - 4)\)
- **Solution:**
  $$
  \begin{aligned}
  &\lim_{x \to 2} (x^2 - 4) \\
  & = (2^2 - 4) \\
  & = (4 - 4) \\
  & = 0
  \end{aligned}
  $$

#### Example 2: Differentiating a Function
- **Problem:** Differentiate \(f(x) = x^3 - 3x^2 + 2x\)
- **Solution:**
  $$
  \begin{aligned}
  &f'(x) = \frac{d}{dx}(x^3 - 3x^2 + 2x) \\
  & = 3x^2 - 6x + 2
  \end{aligned}
  $$

#### Example 3: Integrating a Function
- **Problem:** Integrate \(f(x) = 3x^2 - 4x + 1\)
- **Solution:**
  $$
  \begin{aligned}
  &\int (3x^2 - 4x + 1) \, dx \\
  & = \int 3x^2 \, dx - \int 4x \, dx + \int 1 \, dx \\
  & = x^3 - 2x^2 + x + C
  \end{aligned}
  $$

#### Example 4: Control Systems
- **Problem:** Calculate the integral of the error signal \(e(t) = 3t - 2\) from \(t = 0\) to \(t = 5\) for PID controller tuning.
- **Solution:**
  $$
  \begin{aligned}
  &\int_{0}^{5} (3t - 2) \, dt \\
  & = \left[ \frac{3t^2}{2} - 2t \right]_{0}^{5} \\
  & = \left( \frac{3 \cdot 5^2}{2} - 2 \cdot 5 \right) - \left( \frac{3 \cdot 0^2}{2} - 2 \cdot 0 \right) \\
  & = \left( \frac{75}{2} - 10 \right) - 0 \\
  & = 37.5 - 10 \\
  & = 27.5
  \end{aligned}
  $$

---

## Numerical Methods

### Interpolation
$$
Lagrange \, and \, Newton \, Interpolation
$$

### Numerical Integration
$$
Trapezoidal \, Rule, \, Simpson's \, Rule
$$

### Numerical Differentiation
$$
Forward, \, Backward, \, Central \, Differences
$$

### Applications
- **Simulation**: Numerical methods in finite element analysis (FEA)

### Examples

#### Example 1: Lagrange Interpolation
- **Problem:** Interpolate \(f(x)\) using Lagrange interpolation given \((x_0, y_0) = (1, 1)\), \((x_1, y_1) = (2, 4)\), \((x_2, y_2) = (3, 9)\)
- **Solution:**
  $$
  \begin{aligned}
  &L(x) = \sum_{i=0}^{2} y_i \prod_{\substack{0 \leq j \leq 2 \\ j \neq i}} \frac{x - x_j}{x_i - x_j} \\
  &L(x) = 1 \cdot \frac{(x - 2)(x - 3)}{(1 - 2)(1 - 3)} + 4 \cdot \frac{(x - 1)(x - 3)}{(2 - 1)(2 - 3)} + 9 \cdot \frac{(x - 1)(x - 2)}{(3 - 1)(3 - 2)}
  \end{aligned}
  $$

#### Example 2: Trapezoidal Rule
- **Problem:** Approximate \(\int_{0}^{1} e^x \, dx\) using the trapezoidal rule with \(n = 4\)
- **Solution:**
  $$
  \begin{aligned}
  &\Delta x = \frac{b - a}{n} = \frac{1 - 0}{4} = 0.25 \\
  &x_i = 0, 0.25, 0.5, 0.75, 1 \\
  &\int_{0}^{1} e^x \, dx \approx \frac{\Delta x}{2} [f(x_0) + 2 \sum_{i=1}^{n-1} f(x_i) + f(x_n)] \\
  & \approx \frac{0.25}{2} [e^0 + 2(e^{0.25} + e^{0.5} + e^{0.75}) + e^1] \\
  &\approx \frac{0.25}{2} [1 + 2(1.284 + 1.648 + 2.117) + 2.718] \\
  &\approx \frac{0.25}{2} [1 + 2 \cdot 5.049 + 2.718] \\
  &\approx \frac{0.25}{2} [1 + 10.098 + 2.718] \\
  &\approx \frac{0.25}{2} \cdot 13.816 \\
  &\approx 1.727
  \end{aligned}
  $$

#### Example 3: Central Differences
- **Problem:** Approximate \(f'(x)\) at \(x = 1\) using central differences given \(f(x) = x^2\)
- **Solution:**
  $$
  \begin{aligned}
  &f'(x) \approx \frac{f(x + h) - f(x - h)}{2h} \\
  &

 = \frac{(1.1)^2 - (0.9)^2}{2 \cdot 0.1} \\
  & = \frac{1.21 - 0.81}{0.2} \\
  & = \frac{0.4}{0.2} \\
  & = 2
  \end{aligned}
  $$

#### Example 4: Finite Element Analysis
- **Problem:** Approximate the displacement \(u(x)\) in a beam using numerical methods given boundary conditions \(u(0) = 0\) and \(u(L) = 0\), where \(L = 10\).
- **Solution:**
  Numerical solution using finite element methods will involve discretizing the beam into small elements and applying stiffness matrices. This example would require software tools like MATLAB or ANSYS for detailed steps.

---

## Series

### Arithmetic Series
$$
S_n = \frac{n}{2}(a + l)
$$

### Geometric Series
$$
S_n = a \frac{1 - r^n}{1 - r}
$$

### Taylor Series
$$
f(x) = \sum_{n=0}^{\infty} \frac{f^n(a)}{n!}(x - a)^n
$$

### Applications
- **Digital Signal Processing (DSP)**: Fourier series in signal decomposition

### Examples

#### Example 1: Sum of an Arithmetic Series
- **Problem:** Find the sum of the first 10 terms of the arithmetic series \(1, 3, 5, \ldots\)
- **Solution:**
  $$
  \begin{aligned}
  &a = 1, \quad d = 2, \quad n = 10 \\
  &S_n = \frac{n}{2}(2a + (n - 1)d) \\
  & = \frac{10}{2}(2 \cdot 1 + (10 - 1) \cdot 2) \\
  & = 5(2 + 18) \\
  & = 5 \cdot 20 \\
  & = 100
  \end{aligned}
  $$

#### Example 2: Sum of a Geometric Series
- **Problem:** Find the sum of the first 5 terms of the geometric series \(3, 6, 12, \ldots\)
- **Solution:**
  $$
  \begin{aligned}
  &a = 3, \quad r = 2, \quad n = 5 \\
  &S_n = a \frac{1 - r^n}{1 - r} \\
  & = 3 \frac{1 - 2^5}{1 - 2} \\
  & = 3 \frac{1 - 32}{-1} \\
  & = 3 \cdot 31 \\
  & = 93
  \end{aligned}
  $$

#### Example 3: Taylor Series Expansion
- **Problem:** Find the Taylor series expansion of \(e^x\) around \(x = 0\)
- **Solution:**
  $$
  \begin{aligned}
  &e^x = \sum_{n=0}^{\infty} \frac{x^n}{n!} \\
  & = 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + \cdots
  \end{aligned}
  $$

#### Example 4: DSP - Fourier Series
- **Problem:** Find the Fourier series of \(f(x) = x\) over \([-L, L]\).
- **Solution:**
  $$
  \begin{aligned}
  &f(x) = \sum_{n=1}^{\infty} b_n \sin\left(\frac{n \pi x}{L}\right) \\
  &b_n = \frac{2}{L} \int_{0}^{L} x \sin\left(\frac{n \pi x}{L}\right) dx \\
  &\text{This requires integration by parts and results in:} \\
  &b_n = \frac{2L}{n\pi} \left[(-1)^{n+1}\right]
  \end{aligned}
  $$

---

## Additional Topics

### Transformations
- **Fourier Transform**
$$
F(\omega) = \int_{-\infty}^{\infty} f(t)e^{-j\omega t} \, dt
$$

- **Laplace Transform**
$$
F(s) = \int_{0}^{\infty} f(t)e^{-st} \, dt
$$

- **Z-Transform**
$$
F(z) = \sum_{n=0}^{\infty} f[n]z^{-n}
$$

### Applications
- **Signal Processing**: Fourier transform for frequency analysis

### Examples

#### Example 1: Fourier Transform
- **Problem:** Find the Fourier transform of \(f(t) = e^{-at}\)
- **Solution:**
  $$
  \begin{aligned}
  &F(\omega) = \int_{-\infty}^{\infty} e^{-at}e^{-j\omega t} \, dt \\
  & = \int_{0}^{\infty} e^{-(a+j\omega)t} \, dt \\
  & = \frac{1}{a+j\omega} \quad \text{(for Re}\{a\} > 0)
  \end{aligned}
  $$

#### Example 2: Laplace Transform
- **Problem:** Find the Laplace transform of \(f(t) = t^2\)
- **Solution:**
  $$
  \begin{aligned}
  &F(s) = \int_{0}^{\infty} t^2 e^{-st} \, dt \\
  & = \frac{2}{s^3}
  \end{aligned}
  $$

#### Example 3: Z-Transform
- **Problem:** Find the Z-transform of \(f[n] = n\)
- **Solution:**
  $$
  \begin{aligned}
  &F(z) = \sum_{n=0}^{\infty} n z^{-n} \\
  & = z^{-1} \sum_{n=0}^{\infty} n z^{-n+1} \\
  & = \frac{z^{-1}}{(1 - z^{-1})^2} \\
  & = \frac{z}{(z - 1)^2}
  \end{aligned}
  $$

#### Example 4: Signal Processing
- **Problem:** Calculate the frequency spectrum of a signal \(f(t) = \cos(2\pi f_0 t)\) using Fourier transform.
- **Solution:**
  $$
  \begin{aligned}
  &F(\omega) = \int_{-\infty}^{\infty} \cos(2\pi f_0 t) e^{-j\omega t} \, dt \\
  & = \pi \left[\delta(\omega - 2\pi f_0) + \delta(\omega + 2\pi f_0)\right]
  \end{aligned}
  $$

---

## Key Points and Formulas

### Algebra
1. **Quadratic Formula**: $$(x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}a)$$
2. **Factoring**: $$(a^2 - b^2 = (a + b)(a - b))$$
3. **Binomial Theorem**: $$((a + b)^n = \sum_{k=0}^{n} \binom{n}{k} a^{n-k} b^k)$$
4. **Sum of Arithmetic Series**: $$(S_n = \frac{n}{2} (a + l))$$
5. **Sum of Geometric Series**: $$(S_n = a \frac{1 - r^n}{1 - r})$$

### Trigonometry
1. **Pythagorean Identity**: \(\sin^2(\theta) + \cos^2(\theta) = 1\)
2. **Angle Sum Identities**: \(\sin(a + b) = \sin(a)\cos(b) + \cos(a)\sin(b)\)
3. **Double Angle Formulas**: \(\sin(2\theta) = 2\sin(\theta)\cos(\theta)\), \(\cos(2\theta) = \cos^2(\theta) - \sin^2(\theta)\)
4. **Law of Sines**: \(\frac{\sin(A)}{a} = \frac{\sin(B)}{b} = \frac{\sin(C)}{c}\)
5. **Law of Cosines**: \(c^2 = a^2 + b^2 - 2ab\cos(C)\)

### Linear Algebra
1. **Dot Product**: \(\mathbf{u} \cdot \mathbf{v} = \sum_{i=1}^{n} u_i v_i\)
2. **Cross Product**: \(\mathbf{u} \times \mathbf{v} = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ u_1 & u_2 & u_3 \\ v_1 & v_2 & v_3 \end{vmatrix}\

)
3. **Matrix Determinant**: \(\det(\mathbf{A}) = a_{11}a_{22} - a_{12}a_{21}\)
4. **Eigenvalues and Eigenvectors**: \(\mathbf{A}\mathbf{x} = \lambda \mathbf{x}\)
5. **Matrix Inverse**: \(\mathbf{A}^{-1} = \frac{1}{\det(\mathbf{A})}\text{adj}(\mathbf{A})\)

### Calculus
1. **Chain Rule**: \(\frac{d}{dx} f(g(x)) = f'(g(x))g'(x)\)
2. **Integration by Parts**: \(\int u \, dv = uv - \int v \, du\)
3. **Fundamental Theorem of Calculus**: \(\int_{a}^{b} f(x) \, dx = F(b) - F(a)\)
4. **Taylor Series**: \(f(x) = \sum_{n=0}^{\infty} \frac{f^n(a)}{n!}(x - a)^n\)
5. **L'Hopital's Rule**: \(\lim_{x \to c} \frac{f(x)}{g(x)} = \lim_{x \to c} \frac{f'(x)}{g'(x)}\)

### Numerical Methods
1. **Trapezoidal Rule**: \(\int_{a}^{b} f(x) \, dx \approx \frac{b - a}{2} [f(a) + f(b)]\)
2. **Simpson's Rule**: \(\int_{a}^{b} f(x) \, dx \approx \frac{b - a}{6} [f(a) + 4f\left(\frac{a+b}{2}\right) + f(b)]\)
3. **Newton's Method**: \(x_{n+1} = x_n - \frac{f(x_n)}{f'(x_n)}\)
4. **Euler's Method**: \(y_{n+1} = y_n + h f(x_n, y_n)\)
5. **Runge-Kutta Methods**: \(y_{n+1} = y_n + \frac{h}{6} (k_1 + 2k_2 + 2k_3 + k_4)\), where \(k_i\) are intermediate slopes

---

This comprehensive cheatsheet now includes detailed step-by-step examples for each application and additional key points and formulas, tailored for engineering applications.