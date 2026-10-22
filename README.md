# Incentive Scorecard

A single-page web tool for calculating, tracking and exporting monthly team incentive payouts. Score each team member against a set of KPIs, see their incentive in Rands (ZAR) update live, add them to a team summary, and export everything to Excel or PDF.

## Features

- **Live incentive calculation** – totals update instantly as you select KPI performance bands
- **Multiple KPI categories**, each with its own maximum payout:
  - Individual Performance – Operational KPIs (FCR, Aged Tickets, IVR, USS)
  - Quality Score – QA (10 tickets, scored in Rands per ticket)
  - Team Telephony SLA
  - Opportunities to Exceed (Knowledge Cases, "Pull Right" opportunities)
  - Monthly Knowledge Assessment
  - Compulsory Assessment (compliance-tagged)
- **Core incentive, compliance adjustment and grand total** shown separately
- **Team summary table** to add, review and remove team members
- **Search** for a team member to view their full breakdown
- **Export options**
  - One Excel workbook with a ranked Team Summary sheet plus one sheet per person
  - Individual export per team member
  - PDF export on mobile devices
- **Responsive, dark-themed UI** that works on desktop and mobile

## Getting Started

No build step or installation is needed. It is one self-contained HTML file.

1. Clone or download this repository
2. Open `Incentive_Scorecarda.html` in any modern browser (Chrome, Edge, Firefox, Safari)

An internet connection is required on first load, as the libraries and fonts below are loaded from CDNs.

## How to Use

1. Enter the **team member's name**
2. Select a performance band for each KPI and enter the Rand score for each QA ticket
3. Review the core incentive, compliance adjustment and grand total
4. Click **Add to team summary**
5. Repeat for each team member
6. Click **Export all** to download the results, ranked highest to lowest

## Built With

- HTML, CSS and vanilla JavaScript
- [xlsx-js-style](https://github.com/gitbrent/xlsx-js-style) – styled Excel export
- [JSZip](https://stuk.github.io/jszip/) – file packaging
- [jsPDF](https://github.com/parallax/jsPDF) and [jsPDF-AutoTable](https://github.com/simonbengtsson/jsPDF-AutoTable) – PDF export
- Google Fonts: Sora, Manrope, IBM Plex Mono

## Project Structure

```
.
├── Incentive_Scorecarda.html   # The entire app (markup, styles and logic)
└── README.md
```

## Customising

KPI categories, weightings, maximum payouts and band values are defined in the `categories` configuration inside the `<script>` section of the HTML file. Edit these values to match your own incentive scheme.

## Notes

- Team data is held in the browser session only. Export your results before closing or refreshing the page.
- All amounts are in South African Rand (R).

## Author

Built by Sifiso Kunene.
