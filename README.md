# BLOOMDAY — Your Personal Daily Planner & Journal

A responsive, local-first daily planner built with HTML5, CSS3, and vanilla JavaScript. No backend, build step, API key, or framework is required.

## Run locally

1. Download and unzip `bloomday.zip`.
2. Open the `bloomday` folder in VS Code.
3. Start a local static server (recommended):
   - Install the **Live Server** extension in VS Code.
   - Right-click `index.html` → **Open with Live Server**.
   - Or run `python3 -m http.server 5500` in the project folder and visit `http://localhost:5500`.
4. You can also double-click `index.html`, though browser notifications and clipboard access may require localhost or HTTPS.

## Publish with GitHub Pages

1. Create a GitHub repository (for example `bloomday`).
2. Upload `index.html`, `style.css`, `script.js`, and `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`, then click **Save**.
6. Wait for the deployment and open the URL GitHub Pages displays (usually `https://YOUR-USERNAME.github.io/bloomday/`).

All project asset paths are relative, so the app works from a GitHub Pages project subpath.

## Features

- Dashboard with time-aware greeting, date, daily quote, task progress, habits, and verse.
- Task creation, editing, deletion, completion, categories, priorities, deadlines, filters, sorting, and overdue state.
- Monthly calendar with task, journal, and mood markers.
- Custom habits, daily check-ins, weekly history, and current streaks.
- Journal with seven moods, six reflection prompts, tomorrow's intention, date-based history, and a mood calendar.
- Motivation quote refresh and 30 Bible verses (King James Version / public domain) with short reflections.
- Productivity overview, date-range statistics, and a simple completion chart.
- Light/dark theme, browser reminders, JSON backup export/import, and data clearing confirmation.
- Local storage persistence across refreshes and browser restarts on the same browser/device.

## Data & reminders

Bloomday stores planner information in the browser's `localStorage`. It does not upload your tasks or journal entries to a server. Export a JSON backup before clearing browser data, using private browsing, or switching devices. Restoring a backup replaces the current Bloomday data after confirmation.

Browser reminders require notification permission and are checked while the page is open. Browsers may delay or suppress notifications in background tabs, and reminders are not guaranteed when the browser or page is closed. Task reminders are checked at the task's local deadline time.

## Notes

- Dates use the device's local timezone.
- Bible quotations are from the King James Version (KJV), which is public domain.
- The Google Fonts import is optional; system fallbacks are included if offline.
- For stronger privacy on a shared device, use a separate browser profile and keep exported backups somewhere private.
