# Launch Lab Landing

Premium bilingual landing page for Launch Lab — a Startup as a Service / Product Studio.

## Highlights
- Modern dark premium aesthetic with purple/cyan accents
- Clear conversion flow (problem → solution → process → proof → action)
- Bilingual content (RU/EN) with instant toggle
- Accessible lead form with validation and success state
- Lightweight, no build step required

## Run locally
1. From the project root, start a static server:

```bash
python3 -m http.server 8080
```

2. Open `http://localhost:8080` in your browser.

## Project structure
- `index.html` — page structure and content
- `styles.css` — global styles, layout, and animations
- `main.js` — language switching, scroll reveals, form validation

## Form integrations
The form is built to be easily connected to a backend or automation:
- Replace the mock timeout in `main.js` with a real request.
- Suggested endpoint: `POST /api/lead` with JSON payload.
- On success, the form locks and shows a confirmation state.

## Notes
- Default language follows browser locale (RU if available, otherwise EN).
- Animations respect `prefers-reduced-motion`.
