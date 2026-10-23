# Scientific-cal — Chatpata Prani

A mobile-first scientific calculator inspired by classic scientific calculators such as the Casio fx-991ES PLUS. This is an original implementation, not an official Casio product.

## Run it

Open `index.html` in a modern browser, or host the repository as a static site. No build step or backend is required.

## Included in this initial version

- Responsive scientific-calculator-style display and keypad
- DEG/RAD/GRA angle-mode selector
- Basic arithmetic, powers, roots, factorials, logarithms and trigonometry
- Answer reuse and calculation history
- Scientific-constant quick insert
- Unit conversion for common length, mass, pressure, energy and speed units
- Quadratic/linear equation solver
- Descriptive statistics
- 2×2 matrix determinant and inverse
- Decimal, binary, octal and hexadecimal conversion
- COMP, CMPLX, STAT, BASE-N, EQN, MATRIX, TABLE and VECTOR mode menu

## Important limitations

This is a starter implementation, not yet a complete fx-991ES PLUS emulator. Complex-number arithmetic, true matrix/vector mode workflows, full statistical distributions/regression, equation systems, table generation, fraction/S⇔D conversion, STO/variables, symbolic/numerical calculus, and the full 40-unit conversion catalogue still need implementation and testing. Do not rely on this build for safety-critical or high-stakes calculations.

## Feature roadmap

1. Build a proper expression parser and regression tests (avoid evaluating expressions through JavaScript).
2. Add exact fraction arithmetic and natural textbook display.
3. Implement complete COMP, CMPLX, STAT, BASE-N, EQN, MATRIX, TABLE and VECTOR workflows.
4. Add all documented physical constants and the calculator's complete unit-conversion list.
5. Add offline PWA support and test on small Android screens.
6. Add automated tests for trigonometry, angle modes, precedence, factorials, matrices, statistics and conversions.

## Inspiration and reference projects

The following public projects were reviewed as feature references. This repository does not copy their source code; this initial implementation is independently written.

- [Akhinoor14/fx991exCalculator](https://github.com/Akhinoor14/fx991exCalculator) — broad ClassWiz-style mode and constant/conversion feature set; its README states MIT licensing.
- [Develifture/scientific-calculator](https://github.com/Develifture/scientific-calculator) — offline-first web calculator with graphing, matrices, statistics, regression and equation solving.
- [Casio fx-991ES PLUS product information](https://www.casio.com/in/scientific-calculators/product.FX-991ESPLUS-2BU/1000/) — hardware reference for the target style and modes.

Feature availability and correctness should be verified before claiming parity with a physical calculator.
