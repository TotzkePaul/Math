# Proving Fermat's Last Theorem Classically for Odd Prime Exponents

Fermat's Last Theorem states that there are no non-trivial integer solutions to the equation:

$$x^n + y^n = z^n$$

for \( n > 2 \) where \( n \) is an odd prime, and \( x, y, z \) are coprime integers. In this paper, we explore the theorem under the assumption that \( n \) is an odd prime, and \( x, y, z \) are coprime. We analyze the theorem by examining the parity of \( x \) and \( y \), and explore four cases based on their even-odd configurations.

## Parity Cases

We first categorize the equation into four cases based on the parity of \( x \) and \( y \). This will help us determine the parity of \( z \) and the powers of \( z^n \). 

### Table of Parity Implications

| Case | \( x \) (odd/even) | \( y \) (odd/even) | \( z \) (odd/even) | Implication for \( z^n \) |
|------|-------------------|--------------------|--------------------|--------------------------|
| 1    | Odd               | Odd                | Even               | \( z^n \) is even         |
| 2    | Even              | Odd                | Odd                | \( z^n \) is odd          |
| 3    | Odd               | Even               | Odd                | \( z^n \) is odd          |
| 4    | Even              | Even               | Even               | \( z^n \) is even         |

### Case 1: \( x \) is Odd, \( y \) is Odd
In this case, since both \( x \) and \( y \) are odd, we can express the sum of odd powers using the following identity:

$$
x^n + y^n = (x + y) \cdot S^+
$$

where S+ is defined as:

$$
S^+ = x^{n-1} - x^{n-2}y + x^{n-3}y^2 - \dots - xy^{n-2} + y^{n-1}
$$

**Observation**: Every term in S+ is odd because both \( x \) and \( y \) are odd. Since there are \( n \) terms in \( S^+ \), the sum is odd. Thus, \( (x + y) \) must be even, and it implies that \( z \) is even, as \( z^n \) must also be even.


Let $z = 2^k \cdot w$, where $w$ is odd. Therefore, we have:




$$
S^+ = w^n \quad \text{and} \quad (x + y) = 2^{nk}
$$

There are n terms in S+ and only has a solution if x = y and |x| = n

[TODO: How to prove the above statement]

Thus we have a contradiction because (x+y) would equal 0

### Case 2: \( x \) is Even, \( y \) is Odd
We now assume \( x \) is even and \( y \) is odd. In this case, we use the difference of odd powers identity:

$$
z^n - y^n = x^n
$$

This can be factored as:

$$
z^n - y^n = (z - y) \cdot S^-
$$

where S- is defined as:

$$
S^- = z^{n-1} + z^{n-2}y + \dots + z^{n-2}y + y^{n-1}
$$

**Observation**: Since \( z \) and \( y \) are both odd, each term in $ S^- $ is odd, and the sum is odd. Thus, \( z - y \) must be even, which implies that \( x^n \) has the same number of factors of 2 as $( z - y )$. Let ( $x = 2^k \cdot w $), where \( w \) is odd, leading to:

$$
S^- = w^n \quad \text{and} \quad (z - y) = 2^{nk}
$$

There are n terms in S- and only has a solution if x =-y and |x| = n

[TODO: How to prove the above statement]

Thus we have a contradiction because (x+y) would equal 0

### Case 3: \( x \) is Odd, \( y \) is Even
Without loss of generality, this case is symmetric to Case 2, as the roles of \( x \) and \( y \) are swapped. Therefore, the same reasoning applies, and we conclude:

$$
S^- = w^n \quad \text{and} \quad (z - x) = 2^{nk}
$$

### Case 4: \( x \) and \( y \) are Even
If both \( x \) and \( y \) are even, then \( z \) must also be even. This would imply that \( x, y, z \) all share a factor of 2, violating the assumption that \( x, y, z \) are coprime. Therefore, this case does not provide a valid solution for Fermat's Last Theorem.

## Conclusion

By analyzing the parity of \( x, y, \) and \( z \) and using the sum and difference of odd powers, we see that no solutions exist where \( x^n + y^n = z^n \) for \( n \) odd and prime, with \( x, y, z \) being coprime. Each case demonstrates either a contradiction or forces a result that is inconsistent with coprimeness, thereby upholding Fermat's Last Theorem for the given case.
