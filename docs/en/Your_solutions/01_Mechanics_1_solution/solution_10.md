\# 10. 3D Kinematics Analysis



\## Problem Statement

A point $M$ moves in 3D space according to the position vector:

$$\\vec{r}(t) = (a \\cos(\\omega t), b \\sin(\\omega t), bt)$$

where $a, b, \\omega$ are positive constants.



\---



\## a) Equation of the Point's Trajectory

The trajectory is defined by the coordinates:

1\. $x = a \\cos(\\omega t)$

2\. $y = b \\sin(\\omega t)$

3\. $z = bt$



\### Analysis:

If we look at the $x$ and $y$ coordinates, we can eliminate the trigonometric parameter by rearranging:

$$\\frac{x}{a} = \\cos(\\omega t) \\quad \\text{and} \\quad \\frac{y}{b} = \\sin(\\omega t)$$

Using the identity $\\cos^2\\theta + \\sin^2\\theta = 1$:

$$\\left(\\frac{x}{a}\\right)^2 + \\left(\\frac{y}{b}\\right)^2 = 1$$



\*\*Trajectory Type:\*\* The projection on the $xy$-plane is an \*\*ellipse\*\*. Because the $z$-coordinate increases linearly with time ($z = bt$), the overall 3D trajectory is an \*\*Elliptical Helix\*\*. 



\*Note: if $a=b$, it becomes a standard Circular Helix.\*



\---



\## b) Path Length from $t=0$ to $t=t\_0$

The path length $S$ is the integral of the speed:

$$S = \\int\_{0}^{t\_0} |\\vec{v}(t)| \\, dt$$



\### Step 1: Find Velocity Vector $\\vec{v}(t)$

$$\\vec{v}(t) = \\frac{d\\vec{r}}{dt} = (-a\\omega \\sin(\\omega t), b\\omega \\cos(\\omega t), b)$$



\### Step 2: Calculate Speed $|\\vec{v}(t)|$

$$|\\vec{v}(t)| = \\sqrt{(-a\\omega \\sin(\\omega t))^2 + (b\\omega \\cos(\\omega t))^2 + b^2}$$

$$|\\vec{v}(t)| = \\sqrt{a^2\\omega^2 \\sin^2(\\omega t) + b^2\\omega^2 \\cos^2(\\omega t) + b^2}$$



\### Step 3: Integrate

If $a=b$, the speed is constant. If $a \\neq b$, the integral involves an Elliptic Integral. Assuming the general form:

$$S = \\int\_{0}^{t\_0} \\sqrt{a^2\\omega^2 \\sin^2(\\omega t) + b^2\\omega^2 \\cos^2(\\omega t) + b^2} \\, dt$$



\---



\## c) Python Visualization and Special Cases



\### Special Cases:

1\. \*\*$a = b$\*\*: The trajectory is a \*\*Circular Helix\*\* with a constant radius $a$.

2\. \*\*$b = 0$\*\*: The motion collapses into a 2D \*\*Ellipse\*\* in the $xy$-plane.

3\. \*\*$\\omega = 0$\*\*: The point stays at $(a, 0, bt)$, which is a \*\*Straight Line\*\* parallel to the $z$-axis.



\### Python Code for Trajectory:

```python

import numpy as np

import matplotlib.pyplot as plt



\# Constants

a, b, w = 5, 2, 1

t = np.linspace(0, 20, 500)



\# Coordinates

x = a \* np.cos(w \* t)

y = b \* np.sin(w \* t)

z = b \* t



\# Plotting

fig = plt.figure(figsize=(10, 7))

ax = fig.add\_subplot(111, projection='3d')

ax.plot(x, y, z, label='Elliptical Helix')

ax.set\_xlabel('X axis')

ax.set\_ylabel('Y axis')

ax.set\_zlabel('Z axis')

ax.set\_title('Trajectory of Point M')

plt.legend()

plt.show()

