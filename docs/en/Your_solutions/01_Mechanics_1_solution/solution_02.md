\# Projectile Motion Analysis \& Optimization



This document provides a detailed physical and analytical study of projectile motion, covering differential equations, kinematic calculations, and range optimization.



\---



\## 1. Projectile Motion Task

\*\*Problem:\*\* A projectile is fired from the ground with an initial velocity ($v\_0$) of $100 \\text{ m/s}$ at an angle ($\\theta$) of $37^\\circ$ above the horizontal.



\### A. Differential Equations of Motion

Using Newton's Second Law ($\\vec{F} = m\\vec{a}$), we derive the equations for horizontal ($x$) and vertical ($y$) directions:



\* \*\*Horizontal ($x$):\*\* No air resistance means $F\_x = 0$.

&#x20;   $$\\frac{d^2x}{dt^2} = 0$$

\* \*\*Vertical ($y$):\*\* Gravity acts downward.

&#x20;   $$\\frac{d^2y}{dt^2} = -g$$



\### B. Initial Velocity Components

Decomposing $v\_0$ into its components:

\* $v\_{0x} = 100 \\cos(37^\\circ) \\approx 100(0.8) = 80 \\text{ m/s}$

\* $v\_{0y} = 100 \\sin(37^\\circ) \\approx 100(0.6) = 60 \\text{ m/s}$







\[Image of projectile motion vector decomposition]





\### C. Time of Flight ($T$)

The projectile hits the ground when $y(t) = 0$:

$$0 = v\_{0y}T - \\frac{1}{2}gT^2 \\implies T = \\frac{2v\_{0y}}{g}$$

$$T = \\frac{2(60)}{9.8} \\approx \\mathbf{12.24 \\text{ s}}$$



\### D. Maximum Height ($H$)

Occurs when vertical velocity $v\_y = 0$:

$$H = \\frac{v\_{0y}^2}{2g} = \\frac{60^2}{2(9.8)} \\approx \\mathbf{183.67 \\text{ m}}$$



\### E. Horizontal Range ($R$)

The total distance covered horizontally:

$$R = v\_{0x} \\cdot T = 80 \\cdot 12.24 \\approx \\mathbf{979.2 \\text{ m}}$$



\---



\## 2. Range Optimization

\*\*Problem:\*\* Show analytically that the maximum range $R(\\theta) = \\frac{v\_0^2 \\sin(2\\theta)}{g}$ is achieved at a launch angle of $45^\\circ$.



\### Analytical Proof

To find the maximum range, we differentiate $R(\\theta)$ with respect to $\\theta$ and set it to zero.



1\.  \*\*First Derivative:\*\*

&#x20;   $$\\frac{dR}{d\\theta} = \\frac{v\_0^2}{g} \\frac{d}{d\\theta}\[\\sin(2\\theta)] = \\frac{2v\_0^2 \\cos(2\\theta)}{g}$$



2\.  \*\*Setting to Zero:\*\*

&#x20;   To find the critical point, set $\\frac{dR}{d\\theta} = 0$:

&#x20;   $$\\cos(2\\theta) = 0$$



3\.  \*\*Solving for $\\theta$:\*\*

&#x20;   Since $\\cos(90^\\circ) = 0$:

&#x20;   $$2\\theta = 90^\\circ \\implies \\mathbf{\\theta = 45^\\circ}$$







\### Verification

The second derivative $R''(\\theta) = -\\frac{4v\_0^2 \\sin(2\\theta)}{g}$. At $\\theta = 45^\\circ$, $R''$ is negative, confirming that $45^\\circ$ is a \*\*maximum\*\*.



\---

\*\*Summary of Results\*\*

| Parameter | Value |

| :--- | :--- |

| Initial Velocity | $100 \\text{ m/s}$ |

| Optimal Angle | $45^\\circ$ |

| Flight Time ($37^\\circ$) | $12.24 \\text{ s}$ |

| Max Height ($37^\\circ$) | $183.67 \\text{ m}$ |

