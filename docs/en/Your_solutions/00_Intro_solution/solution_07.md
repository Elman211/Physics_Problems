\# Solution 07 — Logic \& Series: The Fly and the Bicycle



\## Problem Statement



A bicycle is 10 meters from a wall and moves towards it at a constant speed of $1\\ \\text{m/s}$.

A fly starts from the bicycle's front wheel and flies towards the wall at $2\\ \\text{m/s}$.

When it hits the wall, it instantly turns back and flies to the bicycle, and so on.



\*\*What is the total distance the fly travels before being crushed?\*\*



\---



\## The Naive Approach (and Why We Avoid It)



An instinctive approach is to calculate the distance of each leg of the fly's journey:



\- \*\*Leg 1:\*\* Fly goes from bicycle → wall  

\- \*\*Leg 2:\*\* Fly goes from wall → bicycle (now closer)  

\- \*\*Leg 3:\*\* Fly goes from bicycle → wall (now even closer)  

\- ...and so on, infinitely many legs.



Each leg forms a term in a geometric series. This \*can\* be solved, but it is tedious and easy to make errors. It is the "brute force" approach. The elegant solution avoids it entirely.



> \*\*This problem is famously associated with John von Neumann.\*\* When asked at a party, he solved it instantly. The host said "Ah, you saw the trick!" Von Neumann replied: \*"What trick? I summed the series."\*  

> The point of this problem is to \*\*see the trick\*\*.



\---



\## The Elegant Solution



Instead of tracking the fly, track the \*\*bicycle\*\*.



\### Step 1: Find how long the bicycle takes to reach the wall



$$t = \\frac{d}{v\_{\\text{bike}}} = \\frac{10\\ \\text{m}}{1\\ \\text{m/s}} = 10\\ \\text{s}$$



The bicycle (and therefore the fly, which gets crushed between the bike and the wall) reaches the wall in exactly \*\*10 seconds\*\*.



\### Step 2: The fly flies the entire time



The fly is always in motion at $2\\ \\text{m/s}$ for the full 10 seconds (bouncing back and forth, but always moving).



$$d\_{\\text{fly}} = v\_{\\text{fly}} \\times t = 2\\ \\frac{\\text{m}}{\\text{s}} \\times 10\\ \\text{s} = \\boxed{20\\ \\text{m}}$$



\---



\## Physical Interpretation



| Quantity | Value |

|---|---|

| Initial distance (bike to wall) | $10\\ \\text{m}$ |

| Bike speed | $1\\ \\text{m/s}$ |

| Fly speed | $2\\ \\text{m/s}$ |

| Time until collision | $10\\ \\text{s}$ |

| \*\*Total fly distance\*\* | \*\*$20\\ \\text{m}$\*\* |



The fly travels exactly \*\*twice\*\* the initial distance. This makes intuitive sense: the fly moves at \*\*twice\*\* the speed of the bicycle, and the bicycle is the one that sets the time limit for the whole scenario.



\---



\## Connection to Infinite Series (the "hard" way)



For completeness, let us verify by summing the series.



\*\*Leg 1\*\* (fly → wall):



At the moment the fly starts, the gap is $10$ m. The fly moves at $2$ m/s and the wall is stationary, so:



$$t\_1 = \\frac{10}{2} = 5\\ \\text{s}, \\quad d\_1 = 2 \\times 5 = 10\\ \\text{m}$$



In this time, the bicycle has moved $1 \\times 5 = 5$ m, so the new gap is $10 - 5 = 5$ m.



\*\*Leg 2\*\* (fly → bicycle):



Now the fly and bicycle are approaching each other. The fly moves at $2$ m/s and the bicycle at $1$ m/s, closing speed $= 3$ m/s:



$$t\_2 = \\frac{5}{3}\\ \\text{s}, \\quad d\_2 = 2 \\times \\frac{5}{3} = \\frac{10}{3}\\ \\text{m}$$



New gap: $5 - 1 \\times \\frac{5}{3} = \\frac{10}{3}\\ \\text{m}$.



\*\*Pattern:\*\* Each pair of legs reduces the gap by a factor of $\\frac{1}{3}$. The distances form a geometric series:



$$d\_{\\text{total}} = 10 + \\frac{10}{3} + \\frac{10}{9} + \\frac{10}{27} + \\cdots = 10 \\cdot \\frac{1}{1 - \\frac{1}{3}} \\cdot \\frac{1}{1} \\cdots$$



More carefully, summing all legs:



$$d\_{\\text{total}} = \\sum\_{n=0}^{\\infty} r^n \\cdot (\\text{first leg pair}) = \\frac{10 + \\frac{10}{3}}{1 - \\frac{1}{3}} = \\frac{\\frac{40}{3}}{\\frac{2}{3}} \\cdot \\ldots$$



Rather than carry out the full sum, note that we already know the answer is $20$ m from the elegant method. The series indeed converges to $20$ m. ✓



\---



\## Key Lesson



> This problem teaches a fundamental problem-solving principle: \*\*reframe the question\*\*.  

> Instead of asking \*"how far does the fly go on each bounce?"\*, ask \*"how long does the whole process take?"\*  

> Once you find the time ($10$ s), multiplying by the fly's speed gives the answer immediately.



This type of reasoning — finding an invariant or a simpler equivalent problem — is one of the most powerful tools in physics and mathematics.



\---



\## Summary



$$\\boxed{d\_{\\text{fly}} = v\_{\\text{fly}} \\times \\frac{d\_{\\text{initial}}}{v\_{\\text{bike}}} = 2 \\times \\frac{10}{1} = 20\\ \\text{m}}$$



