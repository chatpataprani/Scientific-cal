# Scientific-cal — Chatpata Prani

A mobile-first scientific calculator and mathematics workspace inspired by the capabilities of classic scientific calculators and modern open-source math tools. Original UI and implementation; not affiliated with Casio.

## Project links\n\n- GitHub: https://github.com/chatpataprani\n- Instagram: https://www.instagram.com/chatpataprani/\n- Source repository: https://github.com/chatpataprani/Scientific-cal\n\n## Run locally

Requires Node.js 18+.

```bash
npm install
npm run dev
```

Open the local URL printed by Vite. Build a production version with `npm run build`; preview it with `npm run preview`. Run regression tests with `npm test`.

## Features

- **Calculator UI:** hardware-inspired scientific-calculator body, LCD-style result display, tactile keypad, mode selectors, responsive mobile layout, dark/light themes, and Settings with Chatpata Prani branding plus GitHub/Instagram/project links.\n- **Number tools:** permutations (nPr), combinations (nCr), GCD, LCM, prime checks, rounding, and random values.\n- **Scientific engine:** arithmetic, implicit multiplication, powers, roots, factorials, logarithms, trigonometric and inverse-trigonometric functions, DEG/RAD/GRAD modes, complex values and answer reuse.
- **Calculator memory:** M and saved variables persisted in local storage.
- **History:** saved calculations, reuse previous expressions, clear history and export history to JSON.
- **Complex numbers:** complex arithmetic using `i`, with math.js expression support.
- **Graphing:** plot a function of `x), adjustable x-range, sampled canvas plot.
- **Matrices:** 2×2 determinant, inverse, transpose, add, subtract, multiply and solve a small linear system.
- **Vectors:** 3D addition/subtraction, dot product, cross product, magnitudes and angle.
- **Statistics:** mean, median, modes, range, quartiles, population/sample variance and standard deviation; linear regression and R².
- **Equation solving:** linear/quadratic equations, complex roots and 2-variable linear systems.
- **Numerical calculus:** finite-difference derivative, trapezoidal numerical integration and Newton root search.
- **Function table:** evaluate a function over a selected range and step.
- **BASE-N:** DEC/BIN/OCT/HEX conversion and basic bitwise output.
- **Unit converter:** common length, area, volume, mass, time, speed, pressure, energy, power, force and data units.
- **Physical constants:** a quick reference for common physics constants.
- **Responsive design:** phone, tablet and desktop layouts; dark/light themes; keyboard input.

## Expression examples

| Expression | Meaning |
| --- | --- |
| `sin(30)` in DEG mode | 0.5 |
| `2pi` | implicit multiplication |
| `3(4+1)` | implicit multiplication |
| `sqrt(81)` | square root |
| `(3+4i)*(2-i)` | complex multiplication |
| `x^2` in the graph/table/calculus tools | function of x |

## Project structure

- `index.html` — app entry point
- `src/main.js` — calculator engine, UI and math tools
- `src/style.css` — responsive interface
- `tests/core.test.js` — core math regression tests
- `vite.config.js` — build configuration

The math engine uses the open-source math.js package rather than JavaScript `eval`. The app runs calculations in the browser and does not require a backend or user account. The first install/build needs network access to fetch npm dependencies; a production build can be hosted as static files.

## Important accuracy notes

This is a capable browser-based calculator, **not a cycle-accurate emulator** of any physical calculator. Graphs, numerical derivatives, numerical integration and root finding are approximate. The current matrix UI is limited to 2×2, and the statistics and distributions tools are not a complete replacement for a professional statistics package. The converter includes common units, not every unit from the physical calculator's printed reference panel. Validate important results independently.

## Feature inspiration

The feature set takes inspiration from publicly documented ideas in projects such as [Develifture/scientific-calculator](https://github.com/Develifture/scientific-calculator), [Akhinoor14/fx991exCalculator](https://github.com/Akhinoor14/fx991exCalculator), [JKMMaths/advanced-scientific-calculator](https://github.com/JKMMaths/advanced-scientific-calculator), and [SymvaCAS](https://github.com/kirinonakar/symvacas). Their source code has not been copied wholesale into this repository; this implementation is independently assembled around feature concepts and the math.js library. See each upstream repository's license before reusing any of its source files.

## License

No license has been added to this repository yet. Add a project license before redistributing the application or accepting outside contributions. The math.js dependency retains its own license.
