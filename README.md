# Student Performance Dashboard

This repository hosts an interactive D3.js dashboard for the `student_performance_finalscore.csv` dataset.

Files of interest

- `student_dashboard.html` — The main dashboard (interactive visualizations). Open this file in a browser or serve the folder with a static server.
- `student_performance_finalscore.csv` — Input dataset used by the dashboard.
- `index.html` — Redirects to `student_dashboard.html` (helps GitHub Pages root).

Quick local test

```bash
cd "/Users/rayyan/Desktop/Visual lab project"
python3 -m http.server 8080
# Open http://localhost:8080/student_dashboard.html
```

Enable GitHub Pages (publish to the web)

1. Push the repository to GitHub (already done).
2. In the repository on GitHub go to **Settings** → **Pages**.
3. Under **Source**, choose **Branch: main** and **Folder: /** (root), then click **Save**.
4. Wait a minute; the site will be published.

Public URL examples

- If your GitHub username is `rayyanmehmoodd` and the repository is `sales-data-dashboard`, the site will be available at:

```
https://rayyanmehmoodd.github.io/sales-data-dashboard/
```

This will redirect to `student_dashboard.html` and show the dashboard.

Notes & troubleshooting

- If the dashboard cannot fetch the CSV when opened directly via the `file://` protocol, run a local server (see Quick local test) or host via Pages.
- If you prefer the dashboard at a different path, you can rename `student_dashboard.html` to `index.html` and remove the redirect.
- If you want automatic deployment from a workflow or `gh-pages` branch, I can add a GitHub Actions workflow (requires a personal access token if deploying to `gh-pages`).

Want me to enable an automatic workflow that builds and deploys to GitHub Pages? I can add a GitHub Actions workflow next (it can publish to the repository's Pages branch or docs folder).