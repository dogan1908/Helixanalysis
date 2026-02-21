# Differential-Geometric Analysis of the Conical Helix

**Author:** Dogan Balban  
**Language:** English  
**Format:** LaTeX (PDF output)  
**Status:** Publication-ready preprint

---

## Overview

This repository contains the full LaTeX source of the paper

> **"Differential-Geometric Analysis of the Conical Helix:  
> A Complete Treatment of Curvature, Torsion, Frenet Frame,  
> Arc Length, and Geometric Properties"**

The paper presents a rigorous and self-contained differential-geometric analysis
of the **conical helix** defined by the parametrization

$$
\gamma(\theta) =
\begin{pmatrix}
\dfrac{6}{\pi^2}\,\theta\cos\theta \\[6pt]
\dfrac{6}{\pi^2}\,\theta\sin\theta \\[6pt]
-\dfrac{3}{4} + \dfrac{3}{\pi}\,\theta
\end{pmatrix}, \qquad \theta \geq 0.
$$

The curve is the three-dimensional extension of an **Archimedean spiral** whose
structural constant $a = 6/\pi^2 = 1/\zeta(2)$ arises from an arithmetic
uniqueness argument on the quadratic sequence
$k(n) = \tfrac{1}{6}(2n^2 + 3n + 1)$ (see companion paper below).

---

## Mathematical Content

| Topic | Main Result |
|---|---|
| **Cone equation** | $\gamma$ lies on $z = -\tfrac{3}{4} + \tfrac{\pi}{2}\sqrt{x^2+y^2}$ |
| **Arc length** | Exact closed form via $\operatorname{arcsinh}$, asymptotic $L \sim \frac{a}{2}\theta^2$ |
| **Curvature** | $\kappa(\theta) \sim \pi^2/(6\theta)$ as $\theta\to\infty$ |
| **Torsion** | $\tau(\theta) \sim \pi^3/(12\theta^2)$ as $\theta\to\infty$ |
| **Frenet frame** | $\mathbf{T}$, $\mathbf{N}$, $\mathbf{B}$ computed explicitly |
| **Lancret's theorem** | $\kappa/\tau \sim 2\theta/\pi \not\to \mathrm{const}$ → not a classical helix |
| **Basel connection** | Spiral constant $a = 1/\zeta(2)$ |

---

## Repository Structure

```
conical-helix-analysis/
│
├── conical_helix_analysis.tex   # Main LaTeX source (English, publication-ready)
├── README.md                    # This file
└── LICENSE                      # Creative Commons CC BY 4.0
```

---

## How to Compile

The file requires a standard LaTeX distribution (TeX Live 2020+ or MiKTeX).
Compile with `pdflatex` twice to resolve cross-references:

```bash
pdflatex conical_helix_analysis.tex
pdflatex conical_helix_analysis.tex
```

### Required Packages

All packages are part of standard TeX Live / MiKTeX distributions:

| Package | Purpose |
|---|---|
| `amsmath`, `amssymb`, `amsthm` | Mathematical typesetting and theorem environments |
| `mathtools` | Extended mathematical tools |
| `geometry` | Page layout (A4, 2.5 cm margins) |
| `hyperref` | Hyperlinked cross-references and metadata |
| `cleveref` | Intelligent cross-referencing |
| `booktabs` | Professional-quality tables |
| `float` | Precise figure and table placement |
| `xcolor` | Colored hyperlinks |

---

## Companion Papers

This paper is part of a series on the geometry arising from the quadratic sequence
$k(n) = \tfrac{1}{6}(2n^2+3n+1)$:

1. **D. Balban** (2025). *Differential-Geometric Analysis of the Archimedean Spiral
   $r(\theta) = \frac{6}{\pi^2}\theta$.*  
   Independent mathematical publication.

2. **D. Balban** (2025). *Mathematical Analysis of the Cone
   $z = -\frac{3}{4} + \frac{\pi}{2}r$.*  
   Independent mathematical publication.

3. **D. Balban** (2026). *From the Quadratic Sequence to the Conical Helix:
   Geometric Transformation of Diophantine Structures and Embedding of Primes
   in Three-Dimensional Space.*  
   Independent mathematical publication.  
   *(The number-theoretic derivation of the parametrization studied in this paper.)*

4. **This paper** (2026). *Differential-Geometric Analysis of the Conical Helix.*

---

## Key References

- **do Carmo, M. P.** (2016). *Differential Geometry of Curves and Surfaces.* Dover.
- **Frenet, J. F.** (1852). Sur les courbes à double courbure. *J. Math. Pures Appl.* 17, 437–447.
- **Serret, J. A.** (1851). Sur quelques formules relatives à la théorie des courbes à double courbure. *J. Math. Pures Appl.* 16, 193–207.
- **Lancret, M. A.** (1806). Mémoire sur les courbes à double courbure. *Mém. prés. à l'Institut*, 1, 416–454.
- **Euler, L.** (1740). De summis serierum reciprocarum. *Commentarii Acad. Sci. Petropol.* 7, 123–134.

Full bibliography with annotations is included in the paper.

---

## Mathematical Corrections (Relative to Earlier Drafts)

The following errors in earlier manuscript versions have been corrected:

- **Initial curvature formula** (Proposition 5.1): The formula
  $\kappa(0) = 2\sqrt{a^2+b^2}/(a^2+b^2)^{3/2}$ was missing a factor of $a$
  in the numerator. The correct formula is
  $\kappa(0) = 2a/(a^2+b^2) = 4\pi^2/(3(\pi^2+4)) \approx 0.9488$.

- **Inner product proof** (Lemma 7.1): The proof of $\dot\gamma\cdot\ddot\gamma = a^2\theta$
  now contains all intermediate steps explicitly.

- **Two cone angles** (Remark 2.1): A new remark clarifies that
  $\arctan(\pi/2) \approx 57.52°$ (elevation from horizontal) and
  $\arctan(2/\pi) \approx 32.48°$ (opening half-angle from axis) are complementary
  and both correct — they describe the same cone from different reference directions.

---

## License

This work is licensed under the
[Creative Commons Attribution 4.0 International License (CC BY 4.0)](LICENSE).

You are free to share and adapt this material for any purpose, provided appropriate
credit is given to the author.

---

## Citation

If you use this work, please cite it as:

```
@misc{balban2026helixdiff,
  author  = {Balban, Dogan},
  title   = {Differential-Geometric Analysis of the Conical Helix:
             A Complete Treatment of Curvature, Torsion, Frenet Frame,
             Arc Length, and Geometric Properties},
  year    = {2026},
  note    = {Independent mathematical publication},
  url     = {https://github.com/doganbalban/conical-helix-analysis}
}
```

---

## Contact

For questions, corrections, or collaboration inquiries, please open a GitHub
**Issue** in this repository.
