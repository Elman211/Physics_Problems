\# 3. Path Intersection Analysis



\## Problem Statement

Alice and Bob are moving along paths in a 2D plane defined by the following parametric equations:

\* \*\*Alice:\*\* $A(t) = (2 + t, 8 - 3t)$

\* \*\*Bob:\*\* $B(t) = (2t - 1, 2t + 2)$



We need to determine if they collide (share the same position at the same time $t$) and, if not, find the minimum distance between them.



\---



\## 1. Checking for Collision

For a collision to occur, both the $x$-coordinates and $y$-coordinates must be equal at the \*\*same time\*\* $t$.



\### Set $x\_A(t) = x\_B(t)$:

$$2 + t = 2t - 1$$

$$3 = t$$



\### Verify with $y$-coordinates at $t = 3$:

\* $y\_A(3) = 8 - 3(3) = 8 - 9 = -1$

\* $y\_B(3) = 2(3) + 2 = 6 + 2 = 8$



Since \*\*$-1 \\neq 8$\*\*, Alice and Bob \*\*do not collide\*\*. While their paths might cross at different times, they are never at the same spot simultaneously.



\---



\## 2. Determining Minimum Distance

To find the minimum distance, we define the distance function $D(t)$ using the distance formula:

$$D(t) = \\sqrt{(x\_B - x\_A)^2 + (y\_B - y\_A)^2}$$



\### Step A: Find the relative position vector

$$\\Delta x = (2t - 1) - (2 + t) = t - 3$$

$$\\Delta y = (2t + 2) - (8 - 3t) = 5t - 6$$



\### Step B: Square the distance ($f(t) = D^2$)

To make differentiation easier, we minimize the square of the distance:

$$f(t) = (t - 3)^2 + (5t - 6)^2$$

Expand the terms:

$$f(t) = (t^2 - 6t + 9) + (25t^2 - 60t + 36)$$

$$f(t) = 26t^2 - 66t + 45$$



\### Step C: Find the derivative and solve for $t$

$$f'(t) = 52t - 66$$

Set $f'(t) = 0$:

$$52t = 66 \\implies t = \\frac{66}{52} = \\mathbf{\\frac{33}{26} \\approx 1.27 \\text{ units of time}}$$



\### Step D: Calculate the Minimum Distance

Substitute $t = \\frac{33}{26}$ back into $f(t)$:

$$f(1.27) \\approx 26(1.27)^2 - 66(1.27) + 45 \\approx 3.038$$

$$D\_{min} = \\sqrt{3.038} \\approx \\mathbf{1.74 \\text{ units}}$$



\---



\## Summary of Results

| Event | Occurrence | Details |

| :--- | :--- | :--- |

| \*\*Collision\*\* | No | Coordinates do not match at $t=3$ |

| \*\*Time of Min Distance\*\* | $t \\approx 1.27$ | Calculated via $f'(t)=0$ |

| \*\*Minimum Distance\*\* | $\\approx 1.74$ | Distance units |

