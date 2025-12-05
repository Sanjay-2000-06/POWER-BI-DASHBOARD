# Paris 2024 Olympic Games — Power BI Dashboard
 
Power BI dashboard and datasets for analysis of Paris 2024 Olympic Games — medal tallies, athlete demographics, trends and visualizations.

> Project summary (source): This project integrates Olympic medal and athlete datasets to provide an interactive dashboard for analyzing countries, athletes, medals over time, and gender/age insights. :contentReference[oaicite:1]{index=1}

---

## Contents
- `data/` — raw CSVs used for analysis (athletes, medals, medallists, teams, countries).
- `pbix/` — Power BI report file (`Olympic dashboard.pbix`).
- `pptx/` — presentation exported from the dashboard.
- `docs/screenshots/` — optional screenshots or images of the dashboard.
- `scripts/` — optional ETL/data-cleaning scripts.

---

## Key features
- Medal tally by country (gold / silver / bronze / total)
- Athlete-level analysis (age, gender, sport, event)
- Historical trends across Olympic years
- Country comparisons and top performers
- Future-scope ideas: predictive analytics, medals-per-GDP/per-capita, athlete progression

---

## How to open & view
- **Power BI report:** Open `pbix/Olympic dashboard.pbix` with Power BI Desktop.
- **Data files:** View CSVs in `data/` with Excel, pandas, or any CSV viewer.
- **Presentation:** `pptx/Olympic-Games-Power-BI-Dashboard.pptx` contains slides prepared for presentations.

---

## Notes about large files
Power BI `.pbix` files can be large. If the `.pbix` file is over GitHub's 100 MB limit:
- Use **Git LFS** (Large File Storage) to track `.pbix`.
- Alternatively upload the `.pbix` file as a **Release asset** on GitHub and keep only lightweight exported images / the dataset in the repo.

Example Git LFS usage:
```bash
git lfs install
git lfs track "*.pbix"
git add .gitattributes
git add pbix/Olympic\ dashboard.pbix
git commit -m "Add pbix via Git LFS"
git push origin main
