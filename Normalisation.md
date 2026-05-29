## 2. The Canonical Normalisation

Let *ax² + bx + c = 0* with *a ≠ 0*. Dividing through by *a* and isolating
the leading term yields:

&nbsp;&nbsp;&nbsp;&nbsp;*x² = −(b/a)x − (c/a)*

Define *M = −b/a* and *K = −c/a*, and let *f(x) = x²* and *g(x) = Mx + K*.
The equation becomes:

&nbsp;&nbsp;&nbsp;&nbsp;*f(x) = g(x)* &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*(2.1)*

The roots of the original quadratic are precisely the x-coordinates at which
*f* and *g* coincide — the intersection points of the fixed parabola *y = x²*
and the variable line *y = Mx + K*.

---

**Proposition 2.1 — Canonical Representation**

Every quadratic equation *ax² + bx + c = 0*, with *a ≠ 0*, is equivalent to
the intersection problem *f(x) = g(x)*, where *f(x) = x²* is fixed and
*g(x) = Mx + K* with *M = −b/a* and *K = −c/a*. Conversely, every affine
line *y = Mx + K* corresponds to exactly one monic quadratic equation
*x² − Mx − K = 0*. Hence there exists a bijection between monic quadratic
equations and affine lines in the plane.

*Proof.* The rewriting is a sequence of invertible operations: division by
*a ≠ 0* and rearrangement. The map *(b, c) ↦ (M, K)* is surjective onto ℝ²
and injective on monic equations, establishing the bijection. ∎

---

**Remark 2.2**

Dividing by *a* is not merely an algebraic convenience. It is a normalisation
to a canonical form — the choice to make *y = x²* the invariant object shared
by all quadratic equations. In the standard formulation, every equation
*ax² + bx + c = 0* describes a different parabola. Under the canonical
normalisation, every such equation describes a different line against the same
fixed parabola. All coefficient variation is absorbed into the affine function
*g(x) = Mx + K*. The parabola *y = x²* is the fundamental curve of degree
two — the irreducible nonlinear structure, stripped of everything else.

---

**Remark 2.3 — Extension to Degree n**

The same normalisation applies at every degree. For a polynomial of degree *n*
with leading coefficient *aₙ ≠ 0*, isolating the leading term gives:

&nbsp;&nbsp;&nbsp;&nbsp;*xⁿ = −(aₙ₋₁/aₙ)xⁿ⁻¹ − ⋯ − (a₀/aₙ)*

The fixed curve is *f(x) = xⁿ*. The moving curve *g(x)* has degree *n − 1*.
Roots are x-coordinates of intersections of *f* and *g*. The structure is
identical at every degree. The consequences are developed in Section 7.