# 6. Variable Velocity Analysis

## Problem Statement
An object's velocity is defined by the function:
$$v(t) = t^2 + 2t - 5$$

**Initial Condition:** At $t = 0$, the position $x = 4$.

**Goal:** Determine the object's **position** and **acceleration** at time $t = 3$.

---

## 1. Finding Acceleration at $t = 3$
Acceleration $a(t)$ is the first derivative of velocity with respect to time:
$$a(t) = \frac{dv}{dt}$$

### Step A: Differentiate $v(t)$
$$a(t) = \frac{d}{dt}(t^2 + 2t - 5) = 2t + 2$$

### Step B: Evaluate at $t = 3$
$$a(3) = 2(3) + 2 = 6 + 2 = \mathbf{8 \text{ units/s}^2}$$

---

## 2. Finding Position at $t = 3$
Position $x(t)$ is the integral of velocity with respect to time:
$$x(t) = \int v(t) \, dt$$

### Step A: Find the general position function
$$x(t) = \int (t^2 + 2t - 5) \, dt$$
$$x(t) = \frac{1}{3}t^3 + t^2 - 5t + C$$

### Step B: Solve for the constant $C$ using initial conditions
We know $x(0) = 4$:
$$4 = \frac{1}{3}(0)^3 + (0)^2 - 5(0) + C$$
$$\mathbf{C = 4}$$

So, the specific position function is:
$$x(t) = \frac{1}{3}t^3 + t^2 - 5t + 4$$

### Step C: Evaluate at $t = 3$
$$x(3) = \frac{1}{3}(3)^3 + (3)^2 - 5(3) + 4$$
$$x(3) = \frac{27}{3} + 9 - 15 + 4$$
$$x(3) = 9 + 9 - 15 + 4 = \mathbf{7 \text{ units}}$$

---

## Summary of Results
| Parameter at $t=3$ | Calculation | Result |
| :--- | :--- | :--- |
| **Acceleration** | $a(3) = 2(3) + 2$ | $8 \text{ units/s}^2$ |
| **Position** | $x(3) = 9 + 9 - 15 + 4$ | $7 \text{ units}$ |

### Calculus Note:
To move from velocity to acceleration, we **differentiate**. To move from velocity to position, we **integrate** and apply the initial constant of integration.