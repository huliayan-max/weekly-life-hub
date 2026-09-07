# The Self-Taught EMBA

A 78-week independent-study EMBA curriculum, built as a single self-contained
HTML page you can tick off as you go.

**Live:** https://huliayan-max.github.io/weekly-life-hub/emba/
**Print:** [The-Self-Taught-EMBA.pdf](The-Self-Taught-EMBA.pdf) — 9 pages, A4

## Structure

Eight ten-week blocks, each pairing one *analytical* module with one *judgment*
module, then an eight-week capstone. 15 modules, 61 tracked items, ~624 hours at
roughly 8 hours a week.

| Block | Weeks | Modules |
|---|---|---|
| 1 · Read the numbers | 1–10 | ACC 501 Financial Accounting · DEC 511 Statistics for Decision Making |
| 2 · Price the future | 11–20 | FIN 521 Corporate Finance & Valuation · ECO 505 Managerial Economics |
| 3 · Cost and position | 21–30 | ACC 512 Managerial & Cost Accounting · STR 531 Competitive Strategy |
| 4 · Demand and delivery | 31–40 | MKT 515 Marketing Management · OPS 541 Operations & Supply Chain |
| 5 · People, and the table | 41–50 | LED 551 Leading Organizations · NEG 561 Negotiations |
| 6 · Deals and technology | 51–60 | FIN 575 M&A and Corporate Development · TEC 571 Digital & Technology Strategy |
| 7 · The enterprise view | 61–70 | GOV 581 Governance, Ethics & Enterprise Risk · GLB 585 Global Markets & Country Risk |
| 8 · Put it together | 71–78 | CAP 599 Capstone: A Strategic Audit |

Each module carries an exit standard, its texts, a case or practicum run against
your own employer's numbers, and four or five checkable work items.

## Files

| File | Purpose |
|---|---|
| `index.html` | The tracker. No build step, no dependencies. Progress is stored in `localStorage`, per browser. |
| `print.html` | Print-optimised variant (forced light theme, one block per page) used to generate the PDF. |
| `The-Self-Taught-EMBA.pdf` | Rendered from `print.html` with headless Chrome. |
| `icon.png` | Home-screen icon. |

## Regenerating the PDF

```
chrome --headless=new --no-pdf-header-footer \
  --print-to-pdf=The-Self-Taught-EMBA.pdf print.html
```
