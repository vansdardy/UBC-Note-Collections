# Math Final Summary Note

## Definite Integral

$$
\int_a^b f(x) \dd x
$$

$$
\int_a^b -f(x) \dd x=-\int_a^b f(x) \dd x
$$

Given $f(x)$ defined on $[a,b]$ and $\exists s \in [a,b]$,
$$
\int_a^b f(x) \dd x = \int_a^s f(x) \dd x + \int_s^b f(x) \dd x
$$

### 	Riemann Sum/Integral

- Given $f$ defined on $[a,b]$

  - $n$ subdivisions of equal length
  - approximate each vertical strip using a rectangle
  - $\sum$ Area of strip
  - $n \to \infty$

- $f$ is continuous on $[a,b]$, consider $\int_a^b f(x) \dd x$

  - $n$ strips: $\Delta x=\frac{b-a}{n}$

    - $[x_0, x_1], [x_1, x_2],...,[x_{k-1}, x_k],..,[x_{n-1}, x_n]$

  - consider sample point $x_k^* \in [x_{k-1}, x_k]$ and build rectangle with height $f(x_k^*)$, and area $\Delta x \cdot f(x_k^*)$

  - $$
    S_n=\Delta x \sum_{k=1}^n f(x_k^*)
    $$

  - Possible $x_k^*$

    - Right Riemann sum: $x_k^*=x_k=a+k\Delta x$

      - $$
        R_n = \Delta x\sum_{k=1}^n f(x_k)
        $$

    - Left Riemann sum: $x_k^*=x_{k-1}=a+(k-1)\Delta x$

      - $$
        L_n = \Delta x\sum_{k=1}^n f(x_{k-1})
        $$

    - Midpoint Riemann sum: $x_k^* = \frac{x_{k-1}+x_k}{2}$

      - $$
        M_n = \Delta x\sum_{k=1}^n f(x_k^M)
        $$

    - Trapezoidal Riemann sum

      - $$
        T_n = \Delta x \sum_{k=1}^n \frac{f(x_{k-1})+f(x_k)}{2}
        $$

## Properties of Integral

### 	Definition of Definite Integral

$$
\lim_{n \to \infty} \sum_{k=1}^n f(x_k^*) \Delta x=\int_a^b f(x) \dd x
$$

- If the limit exists, the limit takes the same value $\forall x_k^* \in [x_{k-1},x_k]$

### 	When does $\displaystyle \lim_{n \to \infty} S_n$ exist?

- $f(x)$ is defined on $[a,b]$
  - continuous on $[a,b]$, or,
  - finite number of jump discontinuities
- $f(x)$ is integrable on $[a,b]$

### 	Properties of the Definite Integral

$$
\int_a^b [f(x) \pm g(x)] \dd x=\int_a^b f(x) \dd x \pm \int_a^b g(x) \dd x
$$

$$
\int_a^b k \dd x=k(b-a)
$$

$$
\int_a^b [Af(x) \pm Bg(x)] \dd x=A\int_a^b f(x) \dd x \pm B\int_a^b g(x) \dd x
$$

$$
\int_a^b -f(x) \dd x=-\int_a^b f(x) \dd x
$$

$$
\int_a^a f(x) \dd x=0
$$

$$
\int_a^b f(x) \dd x=\int_a^c f(x) \dd x + \int_c^b f(x) \dd x
$$

### 	Properties of Summation

$$
\sum_{i=1}^n k \cdot x_i = k\sum_{i=1}^n x_i
$$

$$
\sum_{i=1}^n (x_i + y_i) = \sum_{i=1}^n x_i + \sum_{i=1}^n y_i
$$

$$
\sum_{i=a}^n k=k(n-a+1)
$$

$$
\sum_{i=1}^n = \frac{n(n+1)}{2}
$$

### 	Reverse Engineering

- Find $\Delta x$

- $\deg(i)=\deg(n)$

- Guess $a$ and $b$

- Guess $f$

- $$
  \lim_{n \to \infty} \sum_{i=1}^n \frac{i^4}{n^5}=\int_a^{a+1} (x-a)^4dx
  $$

## Fundamental Theorem of Calculus

### 	Definition of Integral Function

​		Given **continuous** function $f$ on $[a,b]$, $\forall x \in [a,b]$, let
$$
F(x)=\int_a^x f(t) \dd t
$$
​		Function composition
$$
F(g(x))=\int_a^{g(x)} f(t) \dd t
$$
​		Derivatives
$$
F'(x)=f(t)
$$

$$
[F(g(x))]'=f(g(x)) \cdot g'(x)
$$

### 	Fundamental Theorem of Calculus

​		Let $f$ be continuous on $I$, $\exists a \in I$

- Part 1: Define $F(x)=\int_a^x f(t) \dd t$ on $I$ $\rightarrow$ $F'(x)=f(x)$ on $I$
- Part 2: $G$ be any antiderivative of $f$ on $I$, then $\forall b \in I$, $\int_a^b f(t) \dd t=G(b)-G(a)$

## Area Between Curves

If $f(x)$ and $g(x)$ are continuous, and $f(x) \ge g(x)$ on $[a,b]$, then the area between curve is
$$
Area=\int_a^b [f(x)-g(x)] \dd x
$$
Depending on the situation, it could be easier to do $\int [f(y)-g(y)] \dd y$

Also make sure the different intervals of different inequality relationships

## Modelling with ODEs

- $\dv{y}{t} = ay+b$
- separable if $y'=g(y)f(t)$
- if separable, $\int \frac{1}{g(y)} \dd y=\int f(t) \dd t$
- IVP: ODE with initial conditions
- Solving an ODE is to find the functions that satisfy the ODE

## Techniques of Integration

### 	Substitution -  Reverse Chain Rule

​		Assume: $f(x)$ and $g(x)$ are continuous, $f(g(x))$ is defined. If $u=g(x)$, then
$$
\int f'g(x) \cdot g'(x) \dd x=\int f'(u) \dd x
$$

$$
\int_a^b f'g(x) \cdot g'(x) \dd x=\int_{g(a)}^{g(b)} f'(u) \dd x
$$

### 	Integration by Parts - Reversing Product Rule

​		If $u$ and $v$ are differentiable, 
$$
\int u \dd v = uv - \int v \dd u, \int_a^b u \dd v = uv \Big|_a^b - \int_a^b v \dd u
$$
​		where $\dd v=\dv{v}{x}\dd x$, and $\dd u=\dv{u}{x}\dd x$.

​		Make sure $\int v \dd u$ can be computed with existing techniques

​		Choosing $u$ and $v$

- easy to either differentiate or integrate
  - $\ln(x)$ is easy to differentiate, not to integrate
  - $\arctan(x)$ is easy to differentiate, not to integrate
  - $\frac{1}{1+x^2}$ is easy to integrate, not to differentiate
  - $e^x, \sin(x), \cos(x),...$

### 	Partial Fraction

$$
\int \frac{a}{bx+c} \dd x=\frac{a}{b}\ln|bx+c|+C
$$

$$
\text{Case 1}: \Delta > 0, \int \frac{dx+e}{ax^2 + bx +c} \dd x=\int (\frac{A}{x-m}+\frac{B}{x-n}) \dd x
$$

$$
\text{Case 2}: \Delta = 0, \int \frac{dx+e}{ax^2 + bx +c} \dd x = \int [\frac{A}{x-m}+\frac{B}{(x-m)^2}] \dd x
$$

$$
\text{Case 3}: \Delta < 0, \text{ complete the square for denominator}
$$

$$
\frac{P(x)}{(x-r)(x-s)(x-t)}=\frac{A}{x-r}+\frac{B}{x-s}+\frac{C}{x-t}, A=\frac{P(r)}{(r-s)(r-t)}, etc
$$

$$
\frac{P(x)}{(x-r)(x^2+bx+c)}=\frac{A}{x-r}+\frac{B}{x^2+bx+c}
$$

$$
\text{By long division}, \frac{P(x)}{Q(x)}=s(x)+\frac{r(x)}{Q(x)}, \text{ if} \deg(P(x))>\deg(Q(x))
$$

### 	Trig Sub

- Trig Integrals
  - $\int \sin(x) \dd x = -\cos(x) + C$
  - $\int \cos(x) \dd x = \sin(x) + C$
  - $\int \sec^2(x) \dd x= \tan(x)+C$
  - $\int \sec(x)\tan(x) \dd x = \sec(x)+C$
  - $\int \tan(x) \dd x=-\ln|\cos(x)|+C$
  - $\int \sec(x) \dd x= \ln|\sec(x)+\tan(x)|+C$
- Trig Identities
  - $\sin^2(x)=\frac{1}{2}(1-\cos(2x))$
  - $\cos^2(x)=\frac{1}{2}(1+\cos(2x))$
  - $\sin(2x)=2\sin(x)\cos(x)$
  - $\cos(2x)=\cos^2(x)-\sin^2(x)$
  - $\sin^2(x)+\cos^2(x)=1$
  - Prosthaphaeresis
    - $\sin(\alpha)+\sin(\beta)=2\sin(\frac{\alpha + \beta}{2})\cos(\frac{\alpha - \beta}{2})$
    - $\sin(\alpha)\cos(\beta)=\frac{1}{2}[\sin(\alpha + \beta)\sin(\alpha - \beta)]$
  - $\sec^2(x)=1+\tan^2(x)$

- $\int \sin^n(x)\cos^m(x) \dd x$
  - $n$ odd, $u=\cos(x) \rightarrow -\int (1+u^2)^{\frac{n-1}{2}}u^m \dd u$
  - $m$ odd, $u=\sin(x) \rightarrow \int u^n (1-u^2)^{\frac{m-1}{2}}\dd u$
  - $m$ and $n$ even, integration of sum of even power of $\sin(x)$
- $\int \sec^m(x)\tan^n(x) \dd x$
  - $\int \sec^2(x) \dd x=\tan(x)+C$
  - $\int \sec(x)\tan(x)dx = \sec(x)+C$

- Trig sub
  - $\sqrt{a^2-x^2} \rightarrow x=a\sin(\theta)$
  - $\sqrt{a^2+x^2} \rightarrow x=a\tan(\theta)$

## Solids

$$
\text{Volume} = \lim_{n \to \infty} \sum_{i=1}^n A(x_i^*)\Delta x=\int_a^b A(x)\dd x
$$

​	Washer: $L \perp$ axis of rotation
$$
\text{Area} = \pi (y_2^2-y_1^2)
$$

$$
\text{Volume} =\int_a^b \pi [(f(x))^2-(g(x))^2] \dd x
$$

​	Cylinder: $L \parallel$ axis of rotation
$$
\text{Area} =2\pi x (y_2 - y_1)
$$

$$
\text{Volume} = \int_a^b 2 \pi x [f(x)-g(x)] \dd x
$$

## Improper Integrals

### 	Type I

​		Let $f$ be continuous on $[a,\infty)$, or $(-\infty, a]$
$$
\int_a^{\infty} f(x) \dd x=\lim_{R \to \infty} \int_a^R f(x)\dd x, \int_{-\infty}^a f(x) \dd x=\lim_{R \to -\infty} \int_R^a f(x) \dd x
$$

- If the limit exists, the integral is convergent
- If the limit DNE, the integral is divergent, if $lim = \pm \infty$, it diverges to $\pm \infty$
- If $f$ is continuous on $[d, \infty)$, s.t. $a \in [d, \infty)$ and $b \in [d, \infty)$, $\int_a^{\infty} f(x) \dd x$ converges $\iff$ $\int_b^{\infty} f(x) \dd x$ converges, since $\int_a^{\infty} f(x) \dd x = \int_a^b f(x) \dd x + \int_a^{\infty} f(x) \dd x$

### 	Type II

​		If $f$ is continuous on $(a, b]$ or $[a, b)$, and $c \in (a, b]$ or $c \in [a, b)$,
$$
\int_a^b f(x) \dd x = \lim_{c \to a^+} \int_c^b f(x) \dd x, \int_a^b f(x) \dd x = \lim_{c \to b^-} \int_a^c f(x) \dd x
$$

### 	Comparison Theorem

​		$-\infty \le a \le b \le \infty$, assume $f$ and $g$ are continuous on $(a,b)$, and $\forall x \in (a,b)$, $0 \le f(x) \le g(x)$,

- If $\int_a^b g(x) \dd x$ is convergent, $\int_a^b f(x) \dd x$ is convergent
- If $\int_a^b f(x)\dd x$ is divergent (to $\infty$), $\int_a^b g(x)\dd x$ is divergent (to $\infty$)

## Continuous Probability

​	Definition: A continuous random variable $X$ is an object that records **outcome** of an experiment as one of a continuous set of values

​	$p(x_1 \le X \le x_2)=\int_{x_1}^{x_2} f(x) \dd x$

​	$f(x)$: Probability Density Function (PDF)

- $f(x) \ge 0$
- $\int_{-\infty}^{\infty} f(x) \dd x = 1$

​	Statistical Tools:

- Mean: $\mu = \int_{-\infty}^{\infty} xf(x)\dd x$
- Variance: $\sigma^2 = \int_{-\infty}^{\infty} (x-\mu)f(x) \dd x$
- Standard deviation: $\sigma = \sqrt{\sigma^2}$
- Expectation: $E(X=x)=\int_{-\infty}^{\infty} xf(x) \dd x$
- $\sigma^2=E(x^2)-\mu^2$

### 	Distributions

- Uniform
  - $f(x)=\frac{1}{b-a}, \forall x \in [a,b]$, $f(x)=0$, otherwise
  - $\mu=\frac{a+b}{2}$, $\sigma^2=\frac{a^2+ab+b^2}{3}-(\frac{a+b}{2})^2$
- Exponential
  - $f(x)=ke^{-kx}, \forall x \in [0,\infty)$, $f(x)=0$, otherwise
  - $\mu=\sigma=\frac{1}{k}$
- Standard
  - $f(x)=\frac{1}{\sqrt{2\pi}}e^{-\frac{x^2}{2}}$
  - $\mu=0$, $\sigma=1$
  - $f_{\mu,\sigma}(x)=\frac{1}{\sigma \sqrt{2 \pi}} e^{-\frac{(x-\mu)^2}{2\sigma^2}}$
  - $\int_{-\infty}^{\infty}e^{-x^2} \dd x=\sqrt{\pi}$

### 	Cumulative Density Function

- Given a PDF, define a CDF

$$
F(t)=\int_{-\infty}^{t}f(x) \dd x
$$

$$
\lim_{t \to \infty} F(t)=1
$$

- Median
  - Uniform: $\frac{a + b}{2}$
  - Exponential: $\frac{\ln2}{k}$
  - Standard: $0$

$$
t \space \text{when} \space F(t)=\frac{1}{2}
$$

## Work

$$
W=\int_a^b F(r) \dd r
$$

​	Can also integrate over time, be flexible regarding which integral to use.

​	Key to find the force $F(r)$ over a small displacement $\Delta r$.

## Sequence and Series

### 	Sequence

- A sequence is an ordered list of real numbers with a first element in the list but no last element.
- A sequence is a function where the domain is set of $\Z^+$
- $a_n = f(n), \forall n \in \Z^+$
- A sequence $a_n$ is said to converge to $L$ ($a_n \to L$) if as $n$ gets larger and larger, $a_n$ gets closer and closer to $L$
- If $a_n$ does not converge, it diverges; if $a_n \to \pm \infty$, then the sequence diverges to $\pm \infty$
- Theorem
  - Suppose $a_n \le c_n \le b_n$, $\displaystyle \lim_{n \to \infty} a_n = \lim_{n \to \infty} b_n = L$, then $\displaystyle \lim_{n \to \infty} c_n = L$
- $n^p \le r^n \le n! \le n^n$
- Rigorous Definition
  - $\forall \epsilon > 0, \exists N \in \Z^+$, if $n \ge N$, $|a_n - L| < \epsilon$
- Every convergent sequence is bounded
- Every bounded increasing sequence is convergent

### 	Series

- Infinite series: A formal sum $a_1 + a_2 + a_3 + ... + a_n + ...$, where $a_1, a_2, a_3, ..., a_n, ...$ is an infinite sequence, written as

- $$
  \sum_{n=1}^{\infty}a_n
  $$

- $n$th partial sum of a series is

- $$
  S_n = \sum_{i=1}^n a_i
  $$

- Therefore,

- $$
  \sum_{i=1}^{\infty}a_i=\lim_{n \to \infty}\sum_{i=1}^n a_i=S
  $$

  - In this case, we say the series converges to that limit $S$

- Geometric Series

  - $$
    \sum_{n=1}^{\infty} ar^{n-1}
    $$

  - If $a=0$, $S=0$

  - If $|r|<1$, $S=\frac{a}{1-r}$

  - If $r \ge 1$ and $a > 0$, diverges to $\infty$

  - If $a < 0$, diverges to $-\infty$

  - If $r = -1$, series diverges

- Telescoping Series

  - $$
    \sum_{n=1}^{\infty} \frac{1}{n(n+1)}
    $$

  - Partial sum: $S_n = 1 - \frac{1}{n+1}$

  - Converges to 1

- Harmonic Series

  - $$
    \sum_{n=1}^{\infty} \frac{1}{n}
    $$

  - Diverges to $\infty$

- p-Series

  - $$
    \sum_{n=1}^{\infty} \frac{1}{n^p}
    $$

  - If $p>1$, converges

  - If $p=1$, harmonic series

  - If $p<1$, diverges

### 	Tests for Convergence and Divergence

- Divergence Test

  - If $\displaystyle \sum_{n=1}^{\infty} a_n$ converges, then $\displaystyle \lim_{n \to \infty} a_n = 0$

- If $a_n \ge 0$ and $S_n$ are bounded, $\sum_n a_n$ converges ($S_n$ is bounded and increasing)

- Integral Test

  - Let $f$ be **continuous**, **non-negative**, and **decreasing**, on some interval $[N, \infty)$
  - Let $a_n = f(n)$
  - Then $\sum_n a_n$ converges $\iff$ $\int_N^{\infty} f(x) \dd x$ converges

- Elementary Comparison Tests

  - Let $\forall n:0\le a_n \le b_n$
  - If $\sum_n b_n$ converges, $\sum_n a_n$ converges
  - If $\sum_n a_n$ diverges to $\infty$, $\sum_n b_n$ diverges to $\infty$
  - If $\sum_n |a_n|$ converges, then $\sum_n a_n$ converges

- Limit Comparison Test

  - Let $a_n$, $b_n$ be infinite sequences, s.t. each $b_n > 0$, and $\displaystyle \lim_{n \to \infty} \frac{a_n}{b_n}=L$, $L$ is finite
    - If $\sum_n b_n$ converges, so does $\sum_n a_n$
    - If $\sum_n a_n$ diverges and $L \ne 0$, so does $\sum_n b_n$

- Ratio Test

  - $$
    \lim_{n \to \infty} |\frac{a_{n+1}}{a_n}| = L
    $$

  - If $L < 1$, the series converges

  - If $L > 1$, the series diverges

  - Otherwise, the series can go either way

- An infinite series $\sum_n a_n$ is absolutely convergent if $\sum_n |a_n|$ converges

  - If $\sum_n a_n$ is absolutely convergent, then $\sum_n a_n$ is convergent, since $\sum_n a_n \le \sum_n |a_n|$
  - An infinite series is **conditionally convergent**, if $\sum_n a_n$ is convergent but $\sum_n |a_n|$ diverges

- Alternating Series Test

  - Let $a_n$ be a sequence, $\forall a_n \ge 0$, $a_n$ is decreasing, $\lim_{n \to \infty} a_n = 0$
    - Then $\sum_n (-1)^{n-1} a_n = a_1 - a_2 + a_3 - a_4 + a_5...$ is convergent

## Power Series

​	Definition: A power series is an object of the form
$$
\sum_{n=0}^{\infty} A_n(x-c)^n=A_0 + A_1(x-c) + A_2(x-c)^2+...
$$
​	$A_n$ is the coefficient, and $c$ is the center
$$
\sum_{n=0}^{\infty} x^n=1+x+x^2+x^3+...=\frac{1}{1-x}, |x|<1
$$
​	Can differentiate and integrate power series
$$
f(x)=\sum_{n=0}^{\infty} A_n(x-c)^n
$$

$$
f'(x)=\sum_{n=0}^{\infty} nA_n(x-c)^{n-1}
$$

$$
\int f(x) \dd x=C + \sum_{n=0}^{\infty} A_n\frac{(x-c)^{n+1}}{n+1}
$$

​	Let $R$ be the radius of convergence, $A=\displaystyle \lim_{n \to \infty} |\frac{A_{n+1}}{A_n}|$, we have $R = \frac{1}{A}$

- $R=\infty$, converges everywhere
- $R=0$, converges only at $x=c$, $\displaystyle \sum_{n=0}^{\infty}A_n (x-c)^n=A_0$

### Taylor Series

$$
f(x)=\sum_{n=0}^{\infty} \frac{f^{(n)}(c)}{n!} (x-c)^n
$$

​	If $f(x)=\displaystyle \sum_{n=0}^{\infty} A_n (x-c)^n$ holds true $\forall x$ in some open interval containing $c$, then that power series is a Taylor Series,
$$
A_n = \frac{f^{(n)}(c)}{n!}
$$
​	This does not indicate that $f(x)=\displaystyle \sum_{n=0}^{\infty} \frac{f^{(n)}(c)}{n!} (x-c)^n$ holds true throughout the radius of convergence.

​	Remainder:
$$
\exists a \in [c, x], R_n(x)=\frac{f^{(n+1)}(a)}{(n+1)!}(x-c)^{n+1}
$$
​	To prove a power series hold for all $x$, just prove $\displaystyle \lim_{n \to \infty} R_n(x) = 0$

​	In a Taylor series, the $n$th derivative is always obtained from the coefficient of the term $x^n$.

​	Function with no analytical solutions to its integral can be expressed in a power series. $\int \frac{\sin(x)}{x} \dd x$

### 	Common Taylor Series

$$
\frac{1}{1-x}=\sum_{n=0}^{\infty}x^n, |x|<1
$$

$$
e^x=\sum_{n=0}^{\infty} \frac{x^n}{n!}
$$

$$
\sin(x)=\sum_{n=0}^{\infty} \frac{(-1)^n}{(2n+1)!} x^{2n+1}
$$

$$
\cos(x)=\sum_{n=0}^{\infty} \frac{(-1)^n}{(2n)!}x^{2n}
$$

