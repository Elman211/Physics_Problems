\# 5. Relative Velocity Analysis



\## Problem Statement

A river flows \*\*East\*\* at $v\_r = 2 \\text{ m/s}$. A boat with a speed of $v\_b = 5 \\text{ m/s}$ in still water wants to travel \*\*directly North\*\* across the river.

\* \*\*River width:\*\* $w = 200 \\text{ meters}$.



\*\*Goal:\*\*

1\. Determine the direction (angle) the boat must head.

2\. Calculate the time required to cross the river.



\---



\## 1. Determining the Heading Angle

To move directly North, the boat must head at an angle $\\theta$ \*\*West of North\*\* so that its eastward component of velocity cancels out the river's eastward flow.



\### Velocity Vector Components:

Let $\\vec{v}\_{br}$ be the velocity of the boat relative to the river, and $\\vec{v}\_r$ be the velocity of the river.

\* $v\_{br, x} = -v\_b \\sin(\\theta)$

\* $v\_{br, y} = v\_b \\cos(\\theta)$

\* $v\_{r, x} = 2 \\text{ m/s}$



For the resultant horizontal velocity to be zero:

$$-v\_b \\sin(\\theta) + v\_{r, x} = 0$$

$$5 \\sin(\\theta) = 2$$

$$\\sin(\\theta) = \\frac{2}{5} = 0.4$$



\*\*Calculation:\*\*

$$\\theta = \\arcsin(0.4) \\approx \\mathbf{23.58^\\circ \\text{ West of North}}$$



\---



\## 2. Calculating the Time to Cross

The time to cross depends on the vertical (Northward) component of the boat's resultant velocity ($v\_{res, y}$).



\### Step A: Find the Resultant Vertical Velocity

$$v\_{res, y} = v\_b \\cos(\\theta)$$

Using the Pythagorean identity $\\cos(\\theta) = \\sqrt{1 - \\sin^2(\\theta)}$:

$$v\_{res, y} = 5 \\cdot \\sqrt{1 - (0.4)^2}$$

$$v\_{res, y} = 5 \\cdot \\sqrt{1 - 0.16} = 5 \\cdot \\sqrt{0.84}$$

$$v\_{res, y} \\approx 5 \\cdot 0.9165 = \\mathbf{4.58 \\text{ m/s}}$$



\### Step B: Calculate Time ($t$)

$$t = \\frac{\\text{width}}{\\text{vertical velocity}}$$

$$t = \\frac{200 \\text{ m}}{4.58 \\text{ m/s}} \\approx \\mathbf{43.67 \\text{ seconds}}$$



\---



\## Summary of Results

| Parameter | Value |

| :--- | :--- |

| \*\*Heading Angle\*\* | $23.58^\\circ$ West of North |

| \*\*Resultant Crossing Speed\*\* | $4.58 \\text{ m/s}$ |

| \*\*Crossing Time\*\* | $43.67 \\text{ s}$ |



\### Physics Note:

Because the boat must "fight" the current by angling upstream, its effective speed across the river is lower than its maximum speed in still water ($4.58 \\text{ m/s}$ vs $5 \\text{ m/s}$).

