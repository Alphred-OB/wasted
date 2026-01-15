# Year Progress Tracker

A minimalist, Apple-inspired single-page experience that visualizes how much of the current year has already slipped away. The app combines real-time data, a GitHub-style day grid, and a rotating set of time-centric quotes to remind visitors that resolutions only matter if we act before the year disappears again.

## Features

- **Live year progress** – Calculates how far through the year we are, with a simplified progress bar and percentage overlay.
- **Server-synced clock** – Fetches the visitor’s local time (AM/PM) via `worldtimeapi.org`, then falls back gracefully to device time.
- **Daily heatmap** – A 53×7 GitHub-inspired grid that highlights completed, current, and future days.
- **Momentum stats** – Quick view of remaining days/weeks/months, plus current day/week numbers and progress through the month/day.
- **Purpose banner** – Surfaces how many days and hours of the year are already gone to reinforce the resolution reminder.
- **Quotes about time** – Rotates through curated quotations that spotlight the cost of wasting time.

## Tech Stack

- **HTML/CSS/JavaScript** only – no build tooling required.
- **Space Grotesk** font from Google Fonts.
- **worldtimeapi.org** for accurate visitor time data.

## Local Setup

1. Clone or download this repository.
2. Open `index.html` directly in your browser.
   - Because the clock calls `worldtimeapi.org`, you may need an internet connection or a simple static server to avoid cross-origin blocks in some browsers (`python -m http.server 8000`).
3. Enjoy the live dashboard and tweak copy/colors in `index.html` as needed.

## Customization

- **Colors & layout** – Adjust CSS variables at the top of `index.html` for new palettes.
- **Quotes** – Edit the `quotes` array in the bottom `<script>` to swap or add time-related quotes.
- **Copy** – Update the hero subtitle or purpose banner text to match your voice or campaign.

## Roadmap Ideas

- Persist daily check-ins to localStorage or a backend.
- Export snapshots for sharing on social media.
- Add notification hooks for milestone moments (25%, 50%, 75% of the year).

## License

This project is released under the MIT License. Feel free to remix it into your own year-tracking reminder.
