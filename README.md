# Logic Gates Playground

Reduzer School's interactive logic-gate simulator, used in the open webinar *Logic Gates: How a Computer Decides* (13 Nov 2026).

Plain HTML, CSS and JavaScript in one file (`index.html`), with no build step and no dependencies. The only external request is Google Fonts (Inter, JetBrains Mono); without it the page falls back to system fonts.

## What it does
- Toggle inputs A and B on AND, OR, NOT, NAND, NOR, XOR and XNOR gates; the live truth table highlights the current row.
- **Half adder**: Sum = A XOR B, Carry = A AND B, shown as binary and decimal.
- **Mystery gate**: a random hidden gate; guests test inputs and guess.

## URL parameters (for presenters)
| Parameter | Effect |
|---|---|
| `?gate=and` … `xnor`, `adder`, `mystery` | open a tab |
| `&a=1&b=0` | preset inputs |
| `&hide=1` | hide the output ("?"), for predict-before-reveal |
| `&demo=1` (`&ms=1600`) | step through every input row automatically |
| `&bare=1` | hide header, tabs and footer (clean screen recordings) |
| `&theme=light` / `dark` | force a colour theme |

## Deploy
Served with GitHub Pages from the `main` branch root. `.nojekyll` makes Pages serve the file as is.

Learn to build software: [reduzer.ac.ke](https://reduzer.ac.ke)
