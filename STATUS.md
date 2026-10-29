# STATUS — Free Insurance Appeal & Medical Bill Dispute Kit

## What was built

A complete "freebies kit" for insurance appeals and medical bill disputes, published by Asdale Dynamics, LLC. Includes Markdown documentation and fillable, printable HTML tools — no account needed, nothing uploaded, everything works locally in the browser.

### Files created

| File | Type | Description |
|------|------|-------------|
| `README.md` | Markdown | Kit overview, how to use, license, about Asdale Dynamics, LLC |
| `LICENSE` | Text | MIT License with exact copyright line: `Copyright (c) 2026 Asdale Dynamics, LLC` |
| `denial-tracker.md` | Markdown | Denial letter tracker with table, common denial reasons, tips, disclaimer |
| `appeal-letter-templates.md` | Markdown | Three appeal letter templates (standard, with provider support, external review) + guidance |
| `eob-checklist.md` | Markdown | Line-by-line EOB checklist (15 items), red flags, next steps, key terms |
| `payment-plan-script.md` | Markdown | Call script for negotiating payment plans, questions to ask, after-call steps |
| `denial-tracker.html` | HTML | Fillable, printable denial tracker table (5 rows, 14 columns) with instructions |
| `appeal-letter.html` | HTML | Fillable, printable three appeal letter templates with blank fields |
| `eob-checklist.html` | HTML | Fillable, printable EOB checklist with yes/no/notes columns |
| `payment-plan.html` | HTML | Fillable, printable payment-plan negotiation script with fields |

All HTML files:
- Self-contained (inline CSS, no external dependencies)
- Fillable inputs that become write-on lines when printed
- Print-optimized CSS (`@media print` hides buttons, shows blank lines)
- "Screen-only" disclaimers and action buttons; "print-only" helper text
- Education-only disclaimer on every page

## How to run / use

1. Open any `.html` file in a modern browser (Chrome, Edge, Firefox, Safari).
2. Fill in the fields directly on screen.
3. Press **Print** (Ctrl+P / Cmd+P) or click the "Save as PDF" button to generate a PDF or print to paper.
4. Blank fields render as ruled lines you can write on by hand.
5. No server, no account, no data leaves your device.

Markdown files can be read directly or converted to PDF/HTML with any Markdown tool (pandoc, VS Code preview, GitHub, etc.).

## Verification results

- **HTML syntax**: All 4 HTML files parsed successfully with Python's `html.parser` — no errors.
- **Git commit**: Clean initial commit on `master` with 10 files, 1118 lines added.
- **License**: MIT LICENSE file contains exact required copyright line: `Copyright (c) 2026 Asdale Dynamics, LLC`.
- **README**: Credits Asdale Dynamics, LLC prominently; includes education-only disclaimer.
- **No secrets**: No API keys, personal data, or credentials in any file.
- **No workflows**: No `.github/workflows` or CI files added.
- **Print test**: Print preview in browser renders correctly — buttons hidden, blank lines visible, tables fit page.

## Known gaps / future improvements

- Only 5 rows in the denial tracker HTML table — could add a "Add row" button (JS) or provide more rows.
- No localStorage persistence — data is lost on reload (by design for privacy, but could be an optional feature).
- No automated test suite (no build step; static HTML only).
- Single-page tools — a combined `index.html` hub linking all tools could be added.
- Accessibility: basic semantic HTML, but could add more ARIA labels and focus styles.
- Mobile print margins may need tuning for some printers.
- No translations — English only.

## Compliance with requirements

- ✅ Markdown + printable HTML for all four tools
- ✅ Fillable, printable, no account needed
- ✅ Education only, not legal advice — disclaimer on every page
- ✅ Credit Asdale Dynamics, LLC in README and all files
- ✅ MIT LICENSE with exact copyright line `Copyright (c) 2026 Asdale Dynamics, LLC`
- ✅ Git initialized and committed (plain message, no Co-authored-by)
- ✅ No push, no remote repos, no publishing
- ✅ No secrets, API keys, personal data
- ✅ No `.github/workflows` files
- ✅ Verified HTML parses, commit succeeds
- ✅ STATUS.md written