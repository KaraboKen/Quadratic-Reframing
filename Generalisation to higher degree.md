## Generalization to Cubic Equations

The Fixed Curve Intercept Method extends naturally to cubic equations. For a cubic of the form

`ax³ + bx² + cx + d = 0` with `a ≠ 0`,

divide by `a` and isolate the cubic term:

`x³ = -(b/a)x² - (c/a)x - (d/a)`

Define:

`P = -b/a`, `Q = -c/a`, `R = -d/a`

Then the equation becomes:

`x³ = Px² + Qx + R`

**Interpretation:**

- **Fixed curve (information):** `y = x³` (a cubic curve, never changes)
- **Moving curve (message):** `y = Px² + Qx + R` (a parabola, degree 2)

The roots of the original cubic are the x‑coordinates where the parabola cuts the fixed cubic.

---

### Example 1: A Cubic with a Line as Message

Take `x³ - 7x - 6 = 0`. Normalising gives `x³ = 7x + 6`.

Here `P = 0`, `Q = 7`, `R = 6`. The moving curve is a **line** (degenerate parabola). The fixed cubic `y = x³` and the line `y = 7x + 6` intersect at three points. Solving `x³ - 7x - 6 = 0` gives roots `x = -2, -1, 3`. Check:

- At `x = -2`: `(-2)³ = -8`, `7(-2)+6 = -8` ✓
- At `x = -1`: `(-1)³ = -1`, `7(-1)+6 = -1` ✓
- At `x = 3`: `27 = 21+6 = 27` ✓

So the line meets the cubic at three points. Their x‑coordinates are the roots.

---

### Example 2: A Cubic with a True Parabola as Message

Take `(x-1)(x-2)(x-3) = x³ - 6x² + 11x - 6 = 0`. Normalising gives:

`x³ = 6x² - 11x + 6`

Here `P = 6`, `Q = -11`, `R = 6`. The moving curve is a parabola `y = 6x² - 11x + 6`. The fixed cubic `y = x³` and this parabola intersect at three points:

`(1,1)`, `(2,8)`, `(3,27)`

Their x‑coordinates `1,2,3` are the roots.

---

### Vieta’s Formulas for Cubics (Geometric Interpretation)

For a cubic `x³ + ax² + bx + c = 0` with roots `r₁, r₂, r₃`, the normalised form `x³ = Px² + Qx + R` gives:

- `P = r₁ + r₂ + r₃` (sum of roots)
- `Q = -(r₁r₂ + r₁r₃ + r₂r₃)` (negative sum of pairwise products)
- `R = r₁r₂r₃` (product of roots)

Thus the parabola’s coefficients directly encode the three elementary symmetric sums of the roots. The geometry reveals the algebra.

---

### How Many Real Roots?

Substituting the moving parabola into the fixed cubic yields a single cubic equation in `x`. Therefore, **at most three real intersections** (roots). This matches the fundamental theorem of algebra for cubics – the geometry already knows the bound.

---

### What About the “Blade” Analogy?

For quadratics, the message was a straight line (one edge). For cubics, the message is a parabola (two edges). A parabola can intersect a cubic in up to three points – that’s why a cubic can have up to three real roots. As degree increases, the message gains more edges, allowing more possible real contacts.

---

### Next: Higher Degrees

The pattern continues for any degree `n`:

- Fix the curve `y = xⁿ` (the information)
- Move a polynomial of degree `n-1` (the message)
- Roots = x‑coordinates of the intersections
- The message’s coefficients give the elementary symmetric sums of the roots (Vieta)
- Maximum number of real intersections = `n`

Thus the Fixed Curve Intercept Method provides a unified geometric lens for all polynomial equations.

---

## Summary for This Section

- Cubics are solved by fixing `y = x³` and moving a parabola.
- The parabola’s coefficients encode Vieta’s formulas.
- The maximum number of real intersections is 3, explaining why a cubic has at most 3 real roots.
- This generalises to any degree `n` (fix `y = xⁿ`, move degree `n-1`).