# Strang ILA4 — Problem Set 6.4 #1 (p. 337), closed 21.11.2026 (= PRML 2.17 part 1)

Source: Strang, *Introduction to Linear Algebra*, 4th ed., Wellesley-Cambridge Press 2009,
ISBN 978-0-9802327-1-4 (PDF in the parent folder). Done for PRML Ch. 2 (§2.3).

> Write A as M + N, symmetric matrix plus skew-symmetric matrix:
> A = [1 2 4; 4 3 0; 8 6 5] = M + N (Mᵀ = M, Nᵀ = −N).
> For any square matrix, M = (A + Aᵀ)/2 and N = ___ add up to A.

Handwritten: [`problem-set-6.4-01-handwritten.png`](problem-set-6.4-01-handwritten.png).

| Part | State |
|---|---|
| The rule M = (A + Aᵀ)/2, N = (A − Aᵀ)/2 | **assisted**: he asked where the book states it ("there is no rule how you divide"); it is not in any section's text, only in this problem statement (M given) and 2.7 #39 (p. 119). I gave both formulas, shown on [1 2; 4 3]. My first answer (steps to check instead of the rule) made him angry; give the rule when he asks for it. |
| M + N = A | assisted: N was the blank the exercise asks for, and I gave it; his check (A + Aᵀ)/2 + (A − Aᵀ)/2 = ½(A + Aᵀ + A − Aᵀ), Aᵀ terms cancel |
| Numbers for the 3×3 | skipped: plan correct |
| Mᵀ = M, Nᵀ = −N | not asked here: the same transpose rules are the core of 2.17 part 2 |

Review: the last line stops at "= ½(…)", should end "= ½·2A = A". Minor.

Check questions (asked 21.11.2026):

- 6.4 #1: why is M = (A + Aᵀ)/2 symmetric for every square A? One line, naming the transpose
  rules used. **Answered 22.11.2026, correct** ([`problem-set-6.4-01-check-handwritten.png`](problem-set-6.4-01-check-handwritten.png)).
  His argument, by entries: row 1 of A + Aᵀ is (A's row 1) + (A's column 1); column 1 of
  A + Aᵀ is (A's column 1) + (A's row 1); same entries, so row = column, i.e. entry (i, j) =
  a_ij + a_ji = entry (j, i). Also noted A must be square for A + Aᵀ to exist.
  Review: the column label first read "A's first row + A's first row"; he fixed it to
  "... + A's first column" on the same page. Then added the transpose form himself:
  ((A + Aᵀ)/2)ᵀ = (Aᵀ + A)/2 = (A + Aᵀ)/2, the last step by commutativity of matrix addition.
  Correct; the rules used, (X + Y)ᵀ = Xᵀ + Yᵀ and (Aᵀ)ᵀ = A, are applied but not named on the page. The ½ doesn't affect symmetry;
  he said it is there so that M + N = A, which is right. Transpose rules not named (he argued by
  entries instead, which is a full proof); the matrix-algebra version (A + Aᵀ)ᵀ = Aᵀ + (Aᵀ)ᵀ uses
  (X + Y)ᵀ = Xᵀ + Yᵀ and (Aᵀ)ᵀ = A.
- 6.2 #1 (asked after the first is answered): A has eigenvalues 2 and ½ with eigenvectors x₁, x₂.
  What are the eigenvalues and eigenvectors of A³ and of A⁻¹, and why, from A = SΛS⁻¹?
  **Answered 22.11.2026, correct** (spoken): from SΛ³S⁻¹ and SΛ⁻¹S⁻¹ the eigenvector matrix S is
  unchanged, only Λ changes, so the eigenvectors stay x₁, x₂ and the eigenvalues are raised to the
  same power; also via Ax = λx (A³x = λ³x). He first thought the question repeated his part (b)
  page; the difference: (b) proves matrix identities, the check asks what they say about the
  eigenpairs. Numbers not stated (A³: 8, 1/8; A⁻¹: ½ on x₁, 2 on x₂: same set {2, ½}, swapped
  vectors). PRML link: Σ⁻¹ has Σ's eigenvectors with eigenvalues 1/λᵢ, (2.48)–(2.49).
