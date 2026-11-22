# Strang ILA4 — Problem Set 2.7 #2 (p. 115), closed 22.11.2026

Source: Strang, *Introduction to Linear Algebra*, 4th ed., Wellesley-Cambridge Press 2009,
ISBN 978-0-9802327-1-4 (PDF in the parent folder). Done for PRML Ch. 2 (§2.3).

> Verify that (AB)ᵀ equals BᵀAᵀ but those are different from AᵀBᵀ: [two 2 by 2 matrices].
> In case AB = BA (not generally true!) how do you prove that BᵀAᵀ = AᵀBᵀ?

Handwritten: [`problem-set-2.7-02-handwritten.png`](problem-set-2.7-02-handwritten.png).

| Part | State |
|---|---|
| Numeric check of (AB)ᵀ = BᵀAᵀ ≠ AᵀBᵀ | **skipped: plan correct** (compute both, compare; routine) |
| If AB = BA, prove BᵀAᵀ = AᵀBᵀ | **solved** (spoken, 22.11): AB = BA ⇒ (AB)ᵀ = (BA)ᵀ ⇒ BᵀAᵀ = AᵀBᵀ, by the product rule on each side |

His work: (AB)ᵀ = BᵀAᵀ; extended to three factors with shapes: A C B of sizes N×M, M×K, K×C
gives R, N×C; (ACB)ᵀ = BᵀCᵀAᵀ of sizes C×K, K×M, M×N gives Rᵀ, C×N. His reason for the order:
the shapes only match in reverse order.

Review: three-factor rule and shapes right (unprompted). The shape argument shows the reversed
order is the only one that *fits* when the matrices are rectangular; it is not why it holds, and for
square matrices AᵀBᵀ fits too but is a different matrix (that is what the numeric part shows). The
reason is entry-wise: ((AB)ᵀ)ᵢⱼ = (AB)ⱼᵢ = row j of A · column i of B (PRML (C.1): "verified by
writing out the indices"). Notation: he used C for a matrix and for a dimension (K × C).

Check question (asked 22.11.2026, pending): for square A and B both BᵀAᵀ and AᵀBᵀ are defined,
so the shapes don't decide. Why is (AB)ᵀ equal to BᵀAᵀ and not to AᵀBᵀ? Answer from what entry
(i, j) of (AB)ᵀ is.
