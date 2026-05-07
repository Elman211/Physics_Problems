\# 7. Elimination of Time and Interpretation of Acceleration



\## Problem Statement

The path of a particle is given by the parametric equations:

$$x(t) = 2t^2, \\quad y(t) = 3t^3$$



\---



\## 1. Eliminate the Parameter $t$

To find the Cartesian equation of the path, we isolate $t$ from one equation and substitute it into the other.



From $x(t) = 2t^2$:

$$t^2 = \\frac{x}{2} \\implies t = \\left(\\frac{x}{2}\\right)^{1/2}$$



Substitute this into $y(t)$:

$$y = 3 \\left\[ \\left(\\frac{x}{2}\\right)^{1/2} \\right]^3$$

$$y = 3 \\left(\\frac{x}{2}\\right)^{3/2}$$



Alternatively, squaring both sides to remove fractional exponents:

$$y^2 = 9 \\left(\\frac{x}{2}\\right)^3 = \\frac{9x^3}{8}$$

\*\*Cartesian Equation:\*\* $\\mathbf{8y^2 = 9x^3}$



\---



\## 2. Trajectory Description

The trajectory is a \*\*semi-cubic parabola\*\*. Since $x = 2t^2$, $x$ is always $\\ge 0$. The curve starts at the origin $(0,0)$ and moves into the first quadrant (for $t > 0$) or fourth quadrant (for $t < 0$).



\---



\## 3. Kinematic Vectors and Magnitudes



\### Velocity $\\vec{v}(t)$ and Magnitude $|\\vec{v}(t)|$

Differentiate the position components with respect to time:

\* $v\_x = \\frac{dx}{dt} = 4t$

\* $v\_y = \\frac{dy}{dt} = 9t^2$



\*\*Velocity Vector:\*\* $\\mathbf{\\vec{v}(t) = (4t)\\hat{i} + (9t^2)\\hat{j}}$



\*\*Magnitude:\*\*

$$|\\vec{v}(t)| = \\sqrt{(4t)^2 + (9t^2)^2} = \\mathbf{\\sqrt{16t^2 + 81t^4}}$$



\### Acceleration $\\vec{a}(t)$ and Magnitude $|\\vec{a}(t)|$

Differentiate the velocity components with respect to time:

\* $a\_x = \\frac{dv\_x}{dt} = 4$

\* $a\_y = \\frac{dv\_y}{dt} = 18t$



\*\*Acceleration Vector:\*\* $\\mathbf{\\vec{a}(t) = 4\\hat{i} + (18t)\\hat{j}}$



\*\*Magnitude:\*\*

$$|\\vec{a}(t)| = \\sqrt{4^2 + (18t)^2} = \\mathbf{\\sqrt{16 + 324t^2}}$$



\---



\## 4. Is the acceleration constant?

\*\*No.\*\* For acceleration to be constant, all its components must be independent of time $t$. While the horizontal acceleration ($a\_x = 4$) is constant, the vertical acceleration ($a\_y = 18t$) depends linearly on time. Therefore, the total acceleration vector \*\*changes over time\*\*.



\---



\## Summary Table

| Property | Expression |

| :--- | :--- |

| \*\*Path Equation\*\* | $y = 3(x/2)^{3/2}$ |

| \*\*Velocity\*\* | $4t\\hat{i} + 9t^2\\hat{j}$ |

| \*\*Acceleration\*\* | $4\\hat{i} + 18t\\hat{j}$ |

| \*\*Constancy\*\* | Non-constant (Time-dependent) |

