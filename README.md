# Marketing KPI Dashboard

An interactive dashboard visualizing marketing performance across channels —
ad spend, ROAS, CAC, and the full conversion funnel — built to reflect the
kind of reporting I built and used in a real marketing role.

**Live demo:**https://lakshmisaikumarramineni-web.github.io/marketing-kpi-dashboard/

## Why I built this

At my current role, I built KPI dashboards from scratch to track ad
performance across Google Ads and other channels — replacing manual
spreadsheet reporting with something the team could check at a glance. This
project recreates that kind of dashboard using illustrative data, since the
real numbers are confidential.

## What it shows

- **Summary KPI cards** — current spend, ROAS, CAC, and conversions at a glance
- **Ad spend by channel** — stacked bar chart across Google Ads, Meta, and Email
- **ROAS trend** — return on ad spend over time
- **CAC trend** — customer acquisition cost over time
- **Conversion funnel** — impressions → clicks → leads → conversions, with
  drop-off rates at each stage
- **Revenue by channel** — grouped bar comparison across channels
- **CAC by channel** — doughnut breakdown of acquisition cost per channel
- **Full monthly data table** — every metric broken down by month and channel

## Tech stack

- Plain HTML/CSS/JS — no framework, no build step
- [Chart.js](https://www.chartjs.org/) for all visualizations
- Built with the help of [Claude Code](https://claude.com/product/claude-code),
  Anthropic's terminal-based AI coding assistant
- Deployed via GitHub Pages — fully static, no backend required

## Data note

All data in this dashboard is **illustrative/mock**, generated to represent
realistic patterns (seasonality, channel mix, ROAS/CAC ranges) rather than
actual figures from any employer. It's structured as a single JS object in
the HTML file, making it easy to swap in real data from a live source.

## What I'd do next (production version)

- Pull live data via the **Google Ads API** and **Meta Marketing API**
  instead of static mock data
- Add a date-range filter and channel-level drill-down
- Cache and refresh data on a schedule (e.g., daily) rather than static load
- Add export-to-PDF for weekly stakeholder reporting

## Running it locally

No installation needed — just open `index.html` in any browser. All data
and charts render client-side.
