# Strang ILA4 — Problem Set 2.7 #19(a) (p. 117), closed 22.11.2026

Source: Strang, *Introduction to Linear Algebra*, 4th ed., Wellesley-Cambridge Press 2009,
ISBN 978-0-9802327-1-4 (PDF in the parent folder). Done for PRML Ch. 2 (§2.3, Ex. 2.17).

> 19 Suppose R is rectangular (m by n) and A is symmetric (m by m).
> (a) Transpose RᵀAR to show its symmetry. What shape is this matrix?

| Part | State |
|---|---|
| Symmetry | **solved** (spoken, at the gym) |
| Shape | **skipped: plan correct** (his method: write the shapes, let the inner ones collapse) |

His work (spoken): (RᵀAR)ᵀ = Rᵀ Aᵀ (Rᵀ)ᵀ = RᵀAᵀR, and Aᵀ = A, so (RᵀAR)ᵀ = RᵀAR.

Review: right; three-factor rule used in the right order, (Rᵀ)ᵀ = R, symmetry of A used once, at
the right place. Shape: his first guess was "m by n"; his own method gives n×m · m×m · m×n = n×n.
It must be square anyway: only a square matrix can equal its transpose.

Check question (asked 22.11.2026): where exactly did you use Aᵀ = A? What would
(RᵀAR)ᵀ be if instead Aᵀ = −A?
**Answered 22.11.2026, correct** (spoken): Aᵀ = A is used when Aᵀ in RᵀAᵀR is replaced by A; with
Aᵀ = −A the transpose is the same product with a minus in front, (RᵀAR)ᵀ = −RᵀAR. He linked it to
PRML 2.17 himself (same pattern with R = x − μ).
