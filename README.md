# Units Converter

A clean, minimal unit conversion web app built with vanilla JavaScript and Tailwind CSS. Supports 9 categories of measurement with conversion history saved to localStorage.

## Preview

> Open `index.html` in any browser — no build step or server required.

## Features

- **9 conversion categories** — Length, Mass, Volume, Temperature, Time, Area, Speed, Data Storage, Energy
- **Swap button** — instantly reverse the from/to unit pair
- **Formula hint** — shows the math behind each conversion below the input
- **Quick conversions** — one-click shortcuts for the most common unit pairs per category
- **Conversion history** — every result is saved to localStorage, persists across sessions, capped at 30 entries
- **No dependencies** — single HTML file, Tailwind loaded via CDN, no build tools

## Tech Stack

| Layer | Choice |
|---|---|
| Markup | HTML5 |
| Styling | Tailwind CSS (CDN) |
| Fonts | DM Sans + DM Mono (Google Fonts) |
| Logic | Vanilla JavaScript |
| Storage | localStorage |

## Getting Started

Clone the repo and open the file directly in your browser:

```bash
git clone https://github.com/paulusesthis/units-converter
cd units-converter
open index.html      # macOS
start index.html     # Windows
xdg-open index.html  # Linux
```

No npm install, no build step, no server needed.

## Project Structure

```
units-converter/
└── index.html      # entire app — markup, styles, and logic in one file
└── README.md
```

## Conversion Categories

| Category | Units |
|---|---|
| Length | km, m, cm, mm, mile, yard, foot, inch, nautical mile |
| Mass | tonne, kg, g, mg, pound, ounce, stone, carat |
| Volume | litre, mL, m³, cm³, gallon, quart, pint, fl oz, cup, tablespoon |
| Temperature | Celsius, Fahrenheit, Kelvin |
| Time | year, month, week, day, hour, minute, second, millisecond |
| Area | km², m², cm², mm², hectare, acre, mi², yd², ft² |
| Speed | km/h, m/s, mph, knot, ft/s |
| Data Storage | bit, byte, KB, MB, GB, TB, PB |
| Energy | joule, kilojoule, calorie, kcal, kWh, BTU, eV |

## How History Works

Every successful conversion is saved to `localStorage` under the key `uc_history`. Entries are stored newest-first and capped at 30. Click **History** in the top-right corner to open the history drawer. Click **Clear all** to wipe the history.

## License

MIT