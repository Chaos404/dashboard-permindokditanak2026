# Dashboard Monitoring — Vercel Loader

Static wrapper for the existing Google Apps Script dashboard. The loader is shown while the iframe initializes and hides on iframe load; a timeout provides a direct-link fallback.

## Deploy
1. Push `index.html`, `vercel.json`, and `README.md` to a GitHub repository.
2. Import that repository into Vercel.
3. Framework Preset: Other. Build Command: leave empty. Output Directory: `.` (or leave default for static files).
4. Deploy.

## Important
The wrapper does not bypass Google Apps Script access restrictions. Ensure the Web App deployment is available to intended viewers. Cross-origin iframe content cannot be inspected by this wrapper, so an iframe `load` event does not guarantee that the Apps Script page rendered successfully.
