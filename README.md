# Expense Tracker (local, no backend)

Client-only web app to record expenses, filter them, visualize trends, and export to CSV. Data is stored in your browser’s localStorage.

## Features
- Add expenses with date, category, description, and amount.
- Filter by date range, category, and text search.
- Totals for all vs. filtered expenses, plus current-month highlight in the hero.
- Delete individual entries, clear all, export filtered list to CSV.
- Charts (Chart.js CDN): doughnut by category and line by month (auto-update with filters).
- Modern dark UI with hero CTA buttons and custom logo mark.
- Works offline—no backend required.

## Getting Started
1) Open `index.html` in a modern browser (Chrome, Edge, Firefox, Safari).
2) Add your expenses in the form; data persists locally.
3) Use filters to refine the list; charts and totals update automatically.
4) Export filtered rows to CSV or clear all data from the UI.

## Development Notes
- Stack: HTML, CSS, vanilla JS—no build step needed.
- Charts: Chart.js via CDN.
- Data persistence: `localStorage` under key `expense-tracker:expenses`.
- To reset data, click “Clear All” in the UI or clear the browser’s localStorage entry for the key above.

## Project Structure
- `index.html` – layout and hero, form, filters, charts, table
- `style.css` – modern dark styling, cards, tables, logo mark
- `app.js` – expense logic, persistence, charts, totals, CSV export

## Future Enhancements (ideas)
- Editable rows instead of delete/re-add.
- Import from CSV.
- PWA install support and optional cloud sync.
- Budget targets and alerts per category.