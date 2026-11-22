# Strang ILA4 — Problem Set 6.2 #1 (p. 307), closed 21.11.2026

Source: Strang, *Introduction to Linear Algebra*, 4th ed., Wellesley-Cambridge Press 2009,
ISBN 978-0-9802327-1-4 (PDF in the parent folder). Done for PRML Ch. 2 (§2.3).

> (a) Factor these two matrices into A = SΛS⁻¹:
> A = [1 2; 0 3] and A = [1 1; 3 3].
> (b) If A = SΛS⁻¹ then A³ = ( )( )( ) and A⁻¹ = ( )( )( ).

Context: §6.1 (eigenvalues from det(A − λI) = 0), §6.2 (diagonalization).

Handwritten: [`problem-set-6.2-01-handwritten-1.png`](problem-set-6.2-01-handwritten-1.png) (first matrix,
eigenpairs), [`problem-set-6.2-01-handwritten-2.png`](problem-set-6.2-01-handwritten-2.png) (first matrix,
SΛS⁻¹ and check), [`problem-set-6.2-01-handwritten-3.png`](problem-set-6.2-01-handwritten-3.png) (second
matrix, eigenpairs), [`problem-set-6.2-01-handwritten-4.png`](problem-set-6.2-01-handwritten-4.png) (part (b)).

Parts:

| Part | State |
|---|---|
| (a) A = [1 2; 0 3] | done, checked |
| (a) A = [1 1; 3 3] | eigenpairs solved (λ = 0, 4); factorisation **skipped: plan correct** (triage: same method as the first matrix; the one new idea, a zero eigenvalue with S still invertible, he discussed in chat) |
| (b) A³ | done by him (expansion SΛS⁻¹SΛS⁻¹SΛS⁻¹ = SΛ³S⁻¹), but **assisted**: I had stated the result in chat first |
| (b) A⁻¹ | done by him: first S⁻¹Λ⁻¹S (wrong order); after the hint (multiply A by it; (XYZ)⁻¹ = Z⁻¹Y⁻¹X⁻¹) he showed (SΛS⁻¹)(SΛ⁻¹S⁻¹) = I, so A⁻¹ = SΛ⁻¹S⁻¹ |

## His work

First matrix, A = [1 2; 0 3]:

det(A − λI) = det [1−λ 2; 0 3−λ] = (1 − λ)(3 − λ) − 0, so λ = 1, λ = 3.

- λ = 1: (A − I)x = [0 2; 0 2]x = 0, x = (1, 0).
- λ = 3: (A − 3I)x = [−2 2; 0 0]x = 0, x = (1, 1).

S = [1 1; 0 1], Λ = [1 0; 0 3], det S = 1, S⁻¹ = [1 −1; 0 1].
SΛS⁻¹ = [1 3; 0 3][1 −1; 0 1] = [1 2; 0 3] = A.

Second matrix, A = [1 1; 3 3]:

det(A − λI) = (1 − λ)(3 − λ) − 3 = λ² − 4λ = λ(λ − 4), so λ = 0, λ = 4.

- λ = 0: x = (1, −1).
- λ = 4: (A − 4I)x = [−3 1; 3 −1]x = 0, x = (1, 3).

## Review notes

- First eigenvector was first written (1, −1), copied from the book's Example 1 instead of
  solved; caught by plugging in ([0 2; 0 2](1, −1) = (−2, −2)). Fixed to (1, 0).
- First S⁻¹ was written [1 1; 0 1]: swapped the diagonal but didn't negate b. Caught by S·S⁻¹ ≠ I.
- Habit given: after each eigenvector check Ax = λx; after each inverse check S·S⁻¹ = I.
- Notation: det(A − λI) = [matrix]. A matrix is not a number; write det[…] or |…|.
- He expanded (1 − λ)(3 − λ) and factored it back. Triangular: eigenvalues = diagonal.
- He wanted to invert A − λI to solve (A − λI)x = 0. At an eigenvalue it is singular; find
  the nullspace instead.
- **Misconception, twice in one session:** "singular = has an inverse" (morning), then
  "dependent columns, so non-singular" (second matrix). Both times corrected; he restated it
  right himself: a non-trivial combination of columns = 0 ⇔ singular. Re-test at §6.5 (a Σ
  with a zero eigenvalue).
- Asked whether the second matrix is "not diagonalizable" because of λ = 0: no. Diagonalizing
  needs S⁻¹ (independent eigenvectors); invertibility of A needs no zero eigenvalue. Two separate
  questions.

Part (b), page 4:

A³ = SΛS⁻¹ SΛS⁻¹ SΛS⁻¹ = SΛ³S⁻¹.
A⁻¹ = S⁻¹Λ⁻¹S.

- A³: the inner S⁻¹S pairs are I; right.
- A⁻¹: wrong order. Check he can run: A·(S⁻¹Λ⁻¹S) = SΛS⁻¹S⁻¹Λ⁻¹S, and S⁻¹S⁻¹ doesn't
  cancel. Rule: (XYZ)⁻¹ = Z⁻¹Y⁻¹X⁻¹, which gives SΛ⁻¹S⁻¹ (same S on the outside as A).
- Fixed (same page, later): (SΛS⁻¹)(SΛ⁻¹S⁻¹) = I, so SΛ⁻¹S⁻¹ = (SΛS⁻¹)⁻¹ = A⁻¹. Verified by
  multiplying, which is the right way to prove an inverse. The old line S⁻¹Λ⁻¹S is still on the
  page, not crossed out.
