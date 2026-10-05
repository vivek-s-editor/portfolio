# Vivek S · Video Editor portfolio

Static site: `index.html` + `vivek.jpg` + `Vivek_S_Resume.pdf`. Hosted free on Netlify, connected to this repo (every commit redeploys).

## Connect Netlify (once)
Netlify → Add new site → Import an existing project → GitHub → `portfolio`. Leave build command and publish directory empty → Deploy. Rename under Site configuration → Change site name (e.g. `vivek-s` → vivek-s.netlify.app).

## Connect the Google Sheet (for adding videos)
1. Google Drive → New → Google Sheets → File → Import → upload `vivek-videos-sheet.csv` → Replace current sheet.
2. File → Share → Publish to web → the sheet tab → Comma-separated values (.csv) → Publish. Copy the link.
3. Edit `index.html`, find `const SHEET_CSV_URL = "";` and paste the link between the quotes. Commit.

## Add a new video
1. Upload to Google Drive → Share → General access: Anyone with the link (Viewer).
2. Add a row to the sheet: Title | Category | Drive link | Client.
3. Categories: Podcasts, Reels, Ads, Theme videos (a new name creates a new tab).
4. Refresh the site. The published sheet can take up to 5 minutes to update.

If a card says "Preview unavailable", the Drive file isn't shared as "Anyone with the link".
