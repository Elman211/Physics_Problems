\# Physics Task: Projectile Motion Analysis



\## Problem Statement

A projectile is fired from the ground with an initial velocity of $v\_0 = 100 \\text{ m/s}$ at an angle of $\\theta = 37^\\circ$ above the horizontal. Assume no air resistance and standard gravity $g = 9.8 \\text{ m/s}^2$.



\---



\## 1. Decomposing Initial Velocity

First, we resolve the initial velocity vector into its horizontal ($x$) and vertical ($y$) components.

\- $v\_{0x} = v\_0 \\cos(\\theta) = 100 \\cos(37^\\circ) \\approx 100 \\times 0.7986 = \\mathbf{80 \\text{ m/s}}$

\- $v\_{0y} = v\_0 \\sin(\\theta) = 100 \\sin(37^\\circ) \\approx 100 \\times 0.6018 = \\mathbf{60 \\text{ m/s}}$



\---



\## 2. Derivation of Differential Equations

Using Newton's Second Law, $\\vec{F} = m\\vec{a}$, where $\\vec{a} = \\frac{d^2\\vec{r}}{dt^2}$.



\### Horizontal Direction ($x$)

Since there is no air resistance, the net force in the horizontal direction is zero ($F\_x = 0$).

$$m \\frac{d^2x}{dt^2} = 0$$

Dividing by mass $m$:

$$\\frac{d^2x}{dt^2} = 0$$

\*This implies that horizontal velocity is constant ($v\_x = v\_{0x}$).\*



\### Vertical Direction ($y$)

The only force acting is gravity, which acts downward (negative direction).

$$m \\frac{d^2y}{dt^2} = -mg$$

Dividing by mass $m$:

$$\\frac{d^2y}{dt^2} = -g$$

\*This implies a constant downward acceleration.\*



\---



\## 3. Kinematic Equations

By integrating the differential equations above twice with respect to time $t$, we get:



1\.  \*\*Horizontal Position:\*\* $x(t) = v\_{0x}t$

2\.  \*\*Vertical Position:\*\* $y(t) = v\_{0y}t - \\frac{1}{2}gt^2$

3\.  \*\*Vertical Velocity:\*\* $v\_y(t) = v\_{0y} - gt$



\---



\## 4. Time of Flight ($T$)

The projectile returns to the ground when the vertical displacement $y(t) = 0$.

$$0 = v\_{0y}T - \\frac{1}{2}gT^2$$

$$0 = T(v\_{0y} - \\frac{1}{2}gT)$$

Ignoring the trivial solution $T=0$ (launch time):

$$T = \\frac{2v\_{0y}}{g} = \\frac{2(60)}{9.8} \\approx \\mathbf{12.24 \\text{ s}}$$



\---



\## 5. Maximum Height ($H$)

Maximum height is reached when the vertical velocity $v\_y = 0$.

$$v\_y = v\_{0y} - gt\_{peak} = 0 \\implies t\_{peak} = \\frac{v\_{0y}}{g}$$

Substitute $t\_{peak}$ into the $y(t)$ equation:

$$H = v\_{0y}\\left(\\frac{v\_{0y}}{g}\\right) - \\frac{1}{2}g\\left(\\frac{v\_{0y}}{g}\\right)^2 = \\frac{v\_{0y}^2}{2g}$$

$$H = \\frac{60^2}{2 \\times 9.8} = \\frac{3600}{19.6} \\approx \\mathbf{183.67 \\text{ m}}$$



\---



\## 6. Horizontal Range ($R$)

The range is the horizontal distance traveled during the total time of flight $T$.

$$R = v\_{0x} \\times T$$

$$R = 80 \\times 12.2449... \\approx \\mathbf{979.59 \\text{ m}}$$



\---



\## 7. Summary of Results

| Parameter | Symbol | Calculation | Result |

| :--- | :--- | :--- | :--- |

| \*\*Initial Velocity\*\* | $v\_0$ | Given | $100 \\text{ m/s}$ |

| \*\*Launch Angle\*\* | $\\theta$ | Given | $37^\\circ$ |

| \*\*Time of Flight\*\* | $T$ | $2v\_{0y} / g$ | $12.24 \\text{ s}$ |

| \*\*Maximum Height\*\* | $H$ | $v\_{0y}^2 / 2g$ | $183.67 \\text{ m}$ |

| \*\*Horizontal Range\*\* | $R$ | $v\_{0x} \\times T$ | $979.59 \\text{ m}$ |

