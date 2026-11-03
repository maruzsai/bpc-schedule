# schedule.balatonpark.com

Static GitHub Pages site for the Balaton Park Circuit **Open Track Day time schedule**. Live at <https://schedule.balatonpark.com/>.

## Rules
- **Everything stays flat at the repo root.** `index.html`, `bpc-logo-white.svg`, `favicon.svg`, `og-image.png`, `CNAME`: no subfolders. Reference assets by bare filename.
- `CNAME` holds exactly one line: `schedule.balatonpark.com`.
- No build step, no npm. Edit `index.html` and push.

## Routine updates
Edit only the block between `<!-- EVENT DATA — edit here -->` and `<!-- /EVENT DATA -->` in `index.html`: the date, weekday and every session row. Row classes: `t` Touristic, `s` Sporty, `info`, `lunch`. Session numbers and times are plain text. If the date changes, also update the description in the `<head>` (`meta description`, `og:description`) and `og-image.png`.

## Files
- `bpc-logo-white.svg`: BPC white-text vector logo (red CIRCUIT line). To update it, replace the file under the same name and keep the viewBox aspect ratio in the `<img width height>` attributes.
- `og-image.png`: 1200×630 share image. Regenerate when the event date changes.
- Printing the page (Ctrl/Cmd+P) gives a one-page A4 white version.
