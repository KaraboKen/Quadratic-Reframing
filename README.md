# Diagonal Cutting
### A geometric reframing of polynomial equations

---

## The Story

Every cook knows there are two ways to cut meat.

The first way: you fix the blade and move the meat into it. An electric carving knife works like this. The blade oscillates in place — vertical, mechanical, invariant. You push the meat horizontally into the motion. The blade doesn't care what you're cutting. It stays where it is. You do the moving.

The second way: the meat stays on the board. You pick up the knife and move it. The cut is diagonal — you're choosing the angle, the pressure, the direction. The meat is fixed. The blade is what travels.

Same result. Same cut. Different grip.

---

## The Mathematics

For two hundred years, we have been teaching quadratic equations the first way.

To solve `ax² + bx + c = 0`, you draw the parabola `y = ax² + bx + c` and find where it crosses the x-axis. The axis is fixed — that's the blade. The parabola is the meat. You push a different parabola into the axis for every new equation. The curve moves. The axis stays still. Roots are where the meat hits the blade.

This works. Nobody disputes it.

But there is another way to hold the tools.

---

Take any quadratic equation. Move every term except `x²` to the right side:

```
x² = Mx + K
```

where `M = -b/a` and `K = -c/a`.

Now look at what you have. The left side — `y = x²` — is a parabola. One parabola. The same parabola for every quadratic equation that has ever existed or will ever exist. It never moves.

The right side — `y = Mx + K` — is a straight line. Its slope and intercept change with every equation. It is the blade. It moves.

The roots of your equation are exactly where the line cuts the fixed parabola.

That's Diagonal Cutting.

---

## What Changes When You Hold It This Way

When you fix the parabola and move the line, things that were hidden become visible.

**Vieta's formulas become geometry.**  
The slope `M` is the sum of the roots. The intercept `K` is the negative product of the roots. You can read Vieta directly off the line — no calculation required.

**The discriminant becomes a picture.**  
- Line cuts the parabola at two points → two real roots → `Δ > 0`  
- Line touches the parabola at exactly one point → one repeated root → `Δ = 0`  
- Line misses the parabola entirely → no real roots → `Δ < 0`

You can see which case you're in before you compute anything.

**The quadratic formula becomes a distance.**  
The roots are symmetric about `x = M/2`. The formula measures the horizontal spread from that centre outward. It is a statement about geometry, not just algebra.

**Complex roots become a gap.**  
When the line misses the parabola, the vertical distance between them at the axis of symmetry is the imaginary part of the complex roots made visible. The roots didn't disappear — they moved off the real line, and you can measure how far.

---

## The Pattern Scales

The same reframing works at every degree.

For a cubic, isolate `x³`. What remains on the right is a quadratic — a parabola. Fix `y = x³`. Move the parabola against it. Roots are intersections.

For a quartic, fix `y = x⁴`. Move a cubic against it.

For degree `n`, fix `y = xⁿ`. Move a degree `n-1` curve. Read the intersections.

The maximum number of intersections is always `n`. That is why a degree-n polynomial has at most n roots. Not because of algebra — because a degree-`n` curve and a degree-`(n-1)` curve can only meet so many times. The geometry states the bound before the algebra does.

This is Bézout's theorem, arrived at from a kitchen analogy.

---

## What This Repository Is

This is an open collection of explorations, visualisations, and notes built around the Diagonal Cutting framework.

We are not claiming new algebra. The roots are still found by the quadratic formula, by factorisation, by completing the square. The algebraic content is classical.

What is new is the grip — the choice of which object stays fixed and which one moves. That choice reorganises what is visible, what is geometric, and what can be taught without calculation.

This repo contains:

- **Interactive visualisations** — the fixed parabola, the moving line, the roots as intersections
- **Parameter space explorations** — the `(M, K)` plane and its parabolic discriminant boundary
- **Pedagogical tools** — Vieta, discriminant, complex roots, and the quadratic formula all expressed geometrically
- **Extensions to higher degrees** — the same pattern applied to cubics, quartics, and beyond
- **Notes on the chain structure** — what happens when you descend level by level, and what each level can and cannot see

---

## Who This Is For

Teachers who want a visual entry point into quadratics that doesn't begin with the formula.

Students who want to understand *why* Vieta's formulas are true, *why* the discriminant has three cases, and *where* complex roots actually live.

Anyone who has ever looked at a quadratic equation and wanted to see it rather than just solve it.

---

## The Core Idea

> Standard method: fix the axis, move the parabola into it.  
> Diagonal Cutting: fix the parabola, move the line against it.  
> Same roots. Different grip. And in the difference — a clearer view of why the roots are where they are.

---

## A Note on Origins

This framework was developed independently in 2026, beginning from the practical question of whether quadratic roots could be read from a fixed curve rather than a moving one. The connection to Bézout's theorem emerged from following the pattern honestly across degrees. The author is not aware of this framing appearing as a primary geometric viewpoint in the expository literature, though prior work in this direction is welcomed.

---

*Open exploration. Not a closed theorem. If you see a new direction, open an issue.*

*Welcome to diagonal cutting.*
