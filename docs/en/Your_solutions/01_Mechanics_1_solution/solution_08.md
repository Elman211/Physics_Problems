\# 8. Circular Motion Analysis



\## Problem Statement

Calculate the centripetal acceleration ($a\_c$) of a person standing on the Earth's equator. 



\*\*Given Data:\*\*

\* \*\*Earth's Radius ($R$):\*\* $6378 \\text{ km} = 6,378,000 \\text{ meters}$

\* \*\*Earth's Rotation Period ($T$):\*\* Approximately 24 hours.



\---



\## 1. Constants and Conversions

To perform the calculation in SI units ($\\text{m/s}^2$), we must convert the rotational period into seconds.



\* \*\*Period ($T$):\*\*

&#x20; $$T = 24 \\text{ hours} \\times 60 \\text{ min/hour} \\times 60 \\text{ sec/min}$$

&#x20; $$T = 86,400 \\text{ seconds}$$



\---



\## 2. Determining Angular Velocity ($\\omega$)

The angular velocity of the Earth is the rate at which it completes one full rotation ($2\\pi$ radians):

$$\\omega = \\frac{2\\pi}{T}$$

$$\\omega = \\frac{2\\pi}{86,400} \\approx 7.272 \\times 10^{-5} \\text{ rad/s}$$



\---



\## 3. Calculating Centripetal Acceleration ($a\_c$)

The formula for centripetal acceleration in terms of angular velocity and radius is:

$$a\_c = \\omega^2 R$$



\### Step-by-Step Calculation:

1\. \*\*Square the angular velocity:\*\*

&#x20;  $$\\omega^2 = (7.272 \\times 10^{-5})^2 \\approx 5.288 \\times 10^{-9} \\text{ rad}^2/\\text{s}^2$$



2\. \*\*Multiply by the radius:\*\*

&#x20;  $$a\_c = (5.288 \\times 10^{-9}) \\times 6,378,000$$

&#x20;  $$a\_c \\approx \\mathbf{0.0337 \\text{ m/s}^2}$$



\---



\## Summary of Results

| Parameter | Value |

| :--- | :--- |

| \*\*Radius ($R$)\*\* | $6,378,000 \\text{ m}$ |

| \*\*Angular Velocity ($\\omega$)\*\* | $7.272 \\times 10^{-5} \\text{ rad/s}$ |

| \*\*Centripetal Acceleration ($a\_c$)\*\* | $\\mathbf{0.0337 \\text{ m/s}^2}$ |



\### Physical Interpretation:

The acceleration due to Earth's gravity ($g$) is approximately $9.8 \\text{ m/s}^2$. The centripetal acceleration at the equator is only about \*\*0.34%\*\* of gravity. This small acceleration is the reason why an object weighs slightly less at the equator than at the poles, as the centripetal acceleration "uses up" a tiny portion of the gravitational pull to keep the object in circular motion.

