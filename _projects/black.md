---
layout: page
title: BLACK
description: Bounded Lᴛʟ sAtisfiability ChecKer
img:
importance:
category: work, solvers
---

[BLACK](https://www.black-sat.org) (short for Bounded Lᴛʟ sAtisfiability ChecKer) is a tool for testing the satisfiability of LTL and LTLf formulas based on the SAT encoding of a one-pass and tree-shaped tableau method. More details can be found in the [GitHub repository](https://github.com/black-sat/black).

## contributions

I've contributed to this project adding the support to the past operators in two ways:

- With a _translation procedure_ which remove the past translating an LTL+Past formula into an equisatisfiable LTL one
- _Extending the direct encoding_ in order to make it cope directly with the past

Other minor contributions are:

- New benchmark families of formulas
- Enhancements in some benchmark suite scripts
- Extension of the test suite (to test the past operators)
- Bugs fix
