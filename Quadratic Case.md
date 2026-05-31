# Fixed Curve Intercept Method – Quadratic Case

## Core Idea

Every quadratic equation can be rewritten so that its roots are the **x‑coordinates of the intersection points** between a **fixed parabola** y = x² and a **moving straight line** y = Mx + K.

The parabola never moves. The line changes with each quadratic.

---

## Normalisation

Given ax² + bx + c = 0 with a ≠ 0:

1. Divide by a:  
   x² + (b/a)x + (c/a) = 0

2. Isolate x²:  
   x² = -(b/a)x - (c/a)

3. Define  
   M = -b/a,    K = -c/a  
   Then  
   x² = Mx + K

---

## Geometric Interpretation

- **Fixed curve (meat):** y = x² (a parabola, always the same)
- **Moving blade (interceptor):** y = Mx + K (a straight line)

The **roots** of the original quadratic are the **x‑coordinates** of the points where the line cuts the parabola.

---

## What the Line Tells You

From the equation x² - Mx - K = 0 we have Vieta’s formulas:

r₁ + r₂ = M,    r₁ · r₂ = -K

- **Slope M** = sum of the roots
- **Intercept K** = negative product of the roots

---

## Discriminant = Cut Width

Δ = M² + 4K

- **Δ > 0** : line cuts the parabola at two distinct points → two real roots.  
  Horizontal distance between the roots = √Δ.

- **Δ = 0** : line is tangent to the parabola → one repeated root (double root).  
  Cut width = 0.

- **Δ < 0** : line misses the parabola → complex roots.  
  The minimum vertical gap between line and parabola is β² = -Δ/4, and the imaginary part of the roots is β.

---

## Geometry of the Chord

The two intersection points are P₁ = (r₁, r₁²) and P₂ = (r₂, r₂²).

- **Midpoint** of the chord:  
  ( (r₁+r₂)/2 , (r₁²+r₂²)/2 ) = ( M/2 , M²/2 + K )  
  The vertical line x = M/2 bisects the chord.

- **Length of the chord:**  
  d = √[(r₂-r₁)² + (r₂²-r₁²)²] = √[Δ·(1+M²)]

- **Tangency condition:** Δ = 0 → chord collapses to a point.

---

## Derivative Connection

The slope of the parabola at any point is 2x. At the midpoint x = M/2:

2·(M/2) = M

which equals the slope of the line. Hence the tangent to the parabola at the midpoint is **parallel to the chord** – a special case of the Mean Value Theorem.

---

## Example

Solve x² - 5x + 6 = 0.

- M = 5, K = -6 → equation: x² = 5x - 6
- Fixed parabola: y = x²  
- Moving line: y = 5x - 6

Intersection: x² = 5x - 6 → x² -5x +6 = 0 → roots x = 2, 3.

Check:  
(2,4) and (3,9) lie on both parabola and line.  
Slope = 5 = 2+3, intercept = -6 = -(2·3).

Discriminant Δ = 25 - 24 = 1, cut width = 1, midpoint = x = 2.5.

---

## Polar Coordinates (Optional Unification)

Using x = r·cosθ, y = r·sinθ:

- Fixed parabola: r = tanθ·secθ
- Moving line: r = K / (sinθ - M·cosθ)

Setting equal gives tan²θ - M·tanθ - K = 0.  
Let t = tanθ → t² - M·t - K = 0, the same quadratic.

Thus tanθ = r₁ or tanθ = r₂.  
**The roots are the tangents of the intersection angles.**

This shows that the LP method works in both Cartesian (roots as distances) and polar (roots as angles) – a true unification.

---

## Summary Table

| Quantity | Cartesian | Polar |
|----------|-----------|-------|
| Fixed curve | y = x² | r = tanθ·secθ |
| Moving curve | y = Mx + K | r = K/(sinθ - M·cosθ) |
| Root condition | x² = Mx + K | tan²θ - M·tanθ - K = 0 |
| Roots appear as | x = r₁, r₂ | tanθ = r₁, r₂ |
| Sum of roots | M | tanθ₁ + tanθ₂ = M |
| Product of roots | -K | tanθ₁·tanθ₂ = -K |
| Discriminant | M²+4K | same |
| Tangency | line touches parabola | one angle, double root |
| Complex roots | line misses (gap) | no real angle |

---

## One‑Sentence Takeaway

> Fix the parabola y = x², move the line y = Mx + K. The roots are where they meet – the line’s slope gives the sum, its intercept gives the negative product, and the discriminant is the cut width.