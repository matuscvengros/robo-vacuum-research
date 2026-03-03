# Robot Vacuum Research Pipeline

A quick experiment in using AI agents to automate consumer research — from raw data to polished deliverables.

## What This Is

My wife asked which robot vacuum we should buy. Instead of opening 40 browser tabs, I built a multi-agent pipeline that:

1. **Gathered research** via separate Gemini and Claude sessions (specs, pricing, reviews)
2. **Synthesised** all findings into a structured overview (Librarian agent)
3. **Verified every claim** against live Australian retailer sites (Pedantic Annoyer agent)
4. **Corrected errors** and produced a professional LaTeX report (Corrector agent)
5. **Generated an interactive HTML presentation** for the final audience (my wife)

~40 minutes, ~100k tokens. 7 products compared, 12 factual errors caught, 18 corrections applied.

## Outputs

| File | Description |
|------|-------------|
| `output/03_final_report.pdf` | 19-page verified comparison report |
| `output/presentation.html` | 11-slide interactive presentation |
| `output/01_librarian_overview.md` | Structured research synthesis |
| `output/02_pedantic_review.md` | Price and spec verification log |

## Tools Used

- **Claude Code** — agent orchestration and pipeline execution
- **Gemini & Claude** — initial research and information gathering
- **XeLaTeX** — PDF report compilation
- **Python** (BeautifulSoup, openpyxl) — source file preprocessing

## License

[MIT](LICENSE)
