# Health Tracker (My Diary)

A simple, responsive **frontend-only** Health Tracker web app to log your daily:

- **Water intake** (ml)
- **Exercise duration** (minutes)
- **Blood sugar level** (mg/dL)

Entries are saved in your browser using **LocalStorage**, so they persist after refresh.

## Demo / Run locally

This is a static project (HTML/CSS/JS). You can run it in any browser.

### Option 1: Open directly

1. Download / clone this repository.
2. Open `index.html` in your browser.

### Option 2: Use a local server (recommended)

Using VS Code:

- Install the **Live Server** extension
- Right-click `index.html` → **Open with Live Server**

Or using Node:

```bash
npx serve
```

## Features

- Add daily health entries (date is auto-filled)
- View entries in a table
- Edit an existing entry
- Delete an entry (with confirmation + small delete animation)
- Data persistence via LocalStorage

## Project structure

- `index.html` — UI layout
- `style.css` — styling
- `script.js` — app logic (CRUD + LocalStorage)

## How it works

- On submit, values are validated (all fields required).
- The current date is saved using `new Date().toLocaleDateString()`.
- Data is stored in LocalStorage under these keys:
  - `date`
  - `water`
  - `exercise`
  - `bloodsugar`

## Tech stack

- HTML
- CSS
- JavaScript (Vanilla)
- Font Awesome (icons via CDN)

## Notes / Known quirks

- Data is stored **only in your browser** (not synced across devices).
- Clearing browser storage will remove all entries.

## License

No license file is currently included. If you'd like, add a `LICENSE` file (e.g., MIT).
