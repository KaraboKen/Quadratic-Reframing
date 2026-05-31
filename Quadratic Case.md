# Fixed Curve Intercept Method – Quadratic Case

## Core Idea

Every quadratic equation can be rewritten so that its roots are the **x‑coordinates of the intersection points** between a **fixed parabola** \(y = x^2\) and a **moving straight line** \(y = Mx + K\).

The parabola never moves. The line changes with each quadratic.

---

## Normalisation

Given \(ax^2 + bx + c = 0\) with \(a \neq 0\):

1. Divide by \(a\):  
   \[
   x^2 + \frac{b}{a}x + \frac{c}{a} = 0
   \]

2. Isolate \(x^2\):  
   \[
   x^2 = -\frac{b}{a}x - \frac{c}{a}
   \]

3. Define  
   \[
   M = -\frac{b}{a}, \qquad K = -\frac{c}{a}
   \]  
   Then  
   \[
   x^2 = Mx + K
   \]

---

## Geometric Interpretation

- **Fixed curve (meat):** \(y = x^2\) (a parabola, always the same)
- **Moving blade (interceptor):** \(y = Mx + K\) (a straight line)

The **roots** of the original quadratic are the **x‑coordinates** of the points where the line cuts the parabola.

---

## What the Line Tells You

From the equation \(x^2 - Mx - K = 0\) we have Vieta’s formulas:

\[
r_1 + r_2 = M, \qquad r_1 r_2 = -K
\]

- **Slope \(M\)** = sum of the roots
- **Intercept \(K\)** = negative product of the roots

---

## Discriminant = Cut Width

\[
\Delta = M^2 + 4K
\]

- **\(\Delta > 0\)** : line cuts the parabola at two distinct points → two real roots.  
  Horizontal distance between the roots = \(\sqrt{\Delta}\).

- **\(\Delta = 0\)** : line is tangent to the parabola → one repeated root (double root).  
  Cut width = 0.

- **\(\Delta < 0\)** : line misses the parabola → complex roots.  
  The minimum vertical gap between line and parabola is \(\beta^2 = -\Delta/4\), and the imaginary part of the roots is \(\beta\).

---

## Geometry of the Chord

The two intersection points are \(P_1 = (r_1, r_1^2)\) and \(P_2 = (r_2, r_2^2)\).

- **Midpoint** of the chord:  
  \[
  \left( \frac{r_1+r_2}{2},\; \frac{r_1^2+r_2^2}{2} \right) = \left( \frac{M}{2},\; \frac{M^2}{2} + K \right)
  \]  
  The vertical line \(x = M/2\) bisects the chord.

- **Length of the chord:**  
  \[
  d = \sqrt{(r_2-r_1)^2 + (r_2^2-r_1^2)^2} = \sqrt{\Delta(1+M^2)}
  \]

- **Tangency condition:** \(\Delta = 0\) → chord collapses to a point.

---

## Derivative Connection

The slope of the parabola at any point is \(2x\). At the midpoint \(x = M/2\):

\[
2\cdot\frac{M}{2} = M
\]

which equals the slope of the line. Hence the tangent to the parabola at the midpoint is **parallel to the chord** – a special case of the Mean Value Theorem.

---

## Example

Solve \(x^2 - 5x + 6 = 0\).

- \(M = 5,\; K = -6\) → equation: \(x^2 = 5x - 6\)
- Fixed parabola: \(y = x^2\)  
- Moving line: \(y = 5x - 6\)

Intersection: \(x^2 = 5x - 6\) → \(x^2 -5x +6 = 0\) → roots \(x = 2,\; 3\).

Check:  
\((2,4)\) and \((3,9)\) lie on both parabola and line.  
Slope = \(5 = 2+3\), intercept = \(-6 = -(2\cdot3)\).

Discriminant \(\Delta = 25 - 24 = 1\), cut width = 1, midpoint = \(x = 2.5\).

---

## Polar Coordinates (Optional Unification)

Using \(x = r\cos\theta,\; y = r\sin\theta\):

- Fixed parabola: \(r = \tan\theta \sec\theta\)
- Moving line: \(r = \dfrac{K}{\sin\theta - M\cos\theta}\)

Setting equal gives \(\tan^2\theta - M\tan\theta - K = 0\).  
Let \(t = \tan\theta\) → \(t^2 - Mt - K = 0\), the same quadratic.

Thus \(\tan\theta = r_1\) or \(\tan\theta = r_2\).  
**The roots are the tangents of the intersection angles.**

This shows that the LP method works in both Cartesian (roots as distances) and polar (roots as angles) – a true unification.

---

## Summary

| Quantity | Cartesian | Polar |
|----------|-----------|-------|
| Fixed curve | \(y = x^2\) | \(r = \tan\theta\sec\theta\) |
| Moving curve | \(y = Mx + K\) | \(r = K/(\sin\theta - M\cos\theta)\) |
| Root condition | \(x^2 = Mx + K\) | \(\tan^2\theta - M\tan\theta - K = 0\) |
| Roots appear as | \(x = r_1, r_2\) | \(\tan\theta = r_1, r_2\) |
| Sum of roots | \(M\) | \(\tan\theta_1 + \tan\theta_2 = M\) |
| Product of roots | \(-K\) | \(\tan\theta_1 \cdot \tan\theta_2 = -K\) |
| Discriminant | \(M^2+4K\) | same |
| Tangency | line touches parabola | one angle, double root |
| Complex roots | line misses (gap) | no real angle |

---

## One‑Sentence Takeaway

> *Fix the parabola \(y=x^2\), move the line \(y=Mx+K\). The roots are where they meet – the line’s slope gives the sum, its intercept gives the negative product, and the discriminant is the cut width.*