# ASI Excellence

Performance-appraisal web app for ASI Connect — single-page app
(`index.html`, vanilla JS) backed by Supabase.

Three appraisal tracks: standard appraisals, Branch Manager monthly
check-ins, and the quarterly Executive Scorecard.

## Run locally
1. `cp config.example.js config.js` and fill in your Supabase Project URL
   and **anon** public key (Project Settings → API).
2. Serve the folder over HTTP, e.g. `py -m http.server 8010`, and open
   `http://127.0.0.1:8010/`.

## Deploy
Pushing to `main` publishes `index.html`, `config.js` and the logo to
GitHub Pages via `.github/workflows/deploy.yml`. The anon key is safe in
the browser; all data access is protected by Supabase Row-Level Security.
