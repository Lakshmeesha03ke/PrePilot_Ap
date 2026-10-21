# PrePilot PWA

A responsive, installable Progressive Web App prototype for placement readiness.

## Features in this prototype
- Mobile-responsive dashboard
- Readiness score calculated from six skill scores
- Editable skill assessment (0–100)
- Recommendations ranked using skill gap and importance weight
- Roadmap based on the current profile
- Demo activity logging
- Browser-local persistence via `localStorage`
- PWA manifest and offline service worker

## Run locally
Open `index.html` in a browser for a quick preview. PWA installation and service worker features require HTTPS or localhost.

For local testing, use VS Code Live Server or run:
```bash
python -m http.server 8000
```
Then open `http://localhost:8000`.

## Deploy on Vercel
1. Create a new GitHub repository named `prepilot`.
2. Upload the contents of this folder (not the outer folder itself) to the repository root.
3. In Vercel, choose **Add New → Project**, import the `prepilot` GitHub repository.
4. Framework preset: **Other**. Build command: leave blank. Output directory: `.` (or leave the default if Vercel detects the static site).
5. Deploy. Open the HTTPS URL on your phone.
6. In Chrome on Android, open the site menu and choose **Install app** or **Add to Home screen**.

## Important prototype limitations
- Demo scores are stored in the current browser/device only. They are not synced between devices.
- There is no real account/login, backend database, AI integration, or server-side validation yet.
- Do not collect real passwords or sensitive student data in this frontend-only prototype.
- Google Fonts are optional styling enhancements; the app's layout works with fallback fonts if unavailable.
