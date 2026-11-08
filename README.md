# Lean30 · Offline Fitness Tracker

A mobile-first nutrition, meal swap, grocery, workout and progress tracker for a Filipino-friendly 30-day plan. No external JavaScript, APIs, fonts, images or accounts are needed.

## Quick start: standalone file

Use `Lean30_Offline_Fitness_Tracker.html` if you want the single-file version. Save it locally on your device and open it in a browser that permits local HTML with JavaScript. **Note:** local-storage behavior for `file://` or `content://` URLs varies by phone/browser. Export backups often. Some in-app previewers restrict local data storage.

## Installable phone app (PWA)

The contents of this ZIP are a Progressive Web App. Host the contents (not the ZIP itself) on an HTTPS website, such as GitHub Pages, retaining the folder layout. Visit the HTTPS URL from Chrome on Android, then use **⋮ > Add to Home screen** or **Install app** (wording varies). Once the site has loaded the service worker and offline cache, it will work without network access.

For a simple GitHub Pages deployment: create a repository, add `index.html`, `manifest.webmanifest`, `service-worker.js`, and both icon files to its root; enable Pages under Settings > Pages with `Deploy from a branch`, branch `main`, root `/`. Open the provided Pages URL in Chrome and add to the home screen. For installation, a valid HTTPS origin is required.

## Using it

- **Today:** rotate through dates, choose swaps in dropdowns, tap `+ Log` only for meals you actually ate. Suggested meals are not pre-logged.
- **Food:** recipe library with ingredients and methods; add social snacks or custom calories, protein and servings.
- **Workout:** the 7-day exercise cycle repeats for 30 days; record workout minutes, effort and notes.
- **Progress:** log weight and waist, and see your weight chart.
- **Pantry & Grocery:** edit currently owned stock; logging a built-in recipe deducts quantities, and swaps are marked based on stock. A pantry-only seven-day suggestion button is provided. The grocery forecast is approximate.
- **Grocery:** aggregates ingredients from 7 upcoming days of selected meals, with a shopping checklist.
- **Settings:** starting date, weight, targets, plus JSON backup import/export and erase.

### Budget design

- Suggested meal subtotal: around 1,200 kcal.
- Flexible social allowance: 300–500 kcal, to reach a **full-day total** of around 1,500–1,700 kcal.
- If no social snacks are eaten, use the rest of the daily calories for regular nutritious food. Do not treat 1,200 as the total-day prescription.
- Protein goal: 120 g/day by default (individual plan 110–130 g/day).

All meal macros and social snack values are estimates. Confirm package nutrition labels and serving sizes, especially for yogurt, canned tuna and milk.

### Data & privacy

All data stays in the browser's local storage on that device; there is no server or account sync. Browser storage deletion can remove all records. Regularly use **Settings > Export JSON backup**. Import restores saved records into the app.

## Choose your own Day 1

On the Today screen, choose any calendar date under **Choose Day 1 of your 30-day plan** and tap **Set start date**. Day 1 always begins Workout A regardless of weekday. Existing logs remain attached to their original calendar dates; changing the start date only re-aligns the planned 30-day cycle. You can also edit it under Settings.
