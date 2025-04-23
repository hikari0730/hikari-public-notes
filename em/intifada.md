# Derivation of the Integrating Factor Method

This note presents the derivation of the **Integrating Factor Method** used to solve first-order linear ordinary differential equations (ODEs).

## 1. General Form

We start with a first-order linear ODE:


$$\frac{dy}{dx} + P(x)y = Q(x)$$


Our goal is to find a general solution for $y(x)$.

## 2. Multiplying by the Integrating Factor

Define the **integrating factor** $\mu(x)$ as:

$$
\mu(x) = e^{\int P(x) \, dx}
$$

Multiplying both sides of the original equation by $\mu(x)$:

$$
\mu(x) \frac{dy}{dx} + \mu(x) P(x) y = \mu(x) Q(x)
$$

The left-hand side becomes the derivative of $\mu(x) y$:

$$
\frac{d}{dx}[\mu(x) y] = \mu(x) Q(x)
$$

## 3. Integration

Now integrate both sides with respect to $x$:

$$
\mu(x) y = \int \mu(x) Q(x) dx + C
$$

Solving for $y$:

$$
y(x) = \frac{1}{\mu(x)} \left( \int \mu(x) Q(x) dx + C \right)
$$

## 4. Summary

The solution to the equation:

$$
\frac{dy}{dx} + P(x)y = Q(x)
$$

is given by:

$$
y(x) = \frac{1}{e^{\int P(x) dx}} \left( \int e^{\int P(x) dx} Q(x) \, dx + C \right)
$$

This completes the derivation of the integrating factor method.

---

**Keywords**: integrating factor, linear differential equation, first-order ODE, exact derivative, general solution.
