#  Penguin Explorer – Dashboard by Kiruthikaa

This repository contains the local and client-side deployment of an interactive PyShiny dashboard. It explores data from the `palmerpenguins` dataset with reactive inputs, visualizations, and download functionality — all built with Python and hosted for free via GitHub Pages.

---

## Live Dashboard

View the hosted app here:  
➡️ [https://kiruthikaa2512.github.io/cintel-04-local/](https://kiruthikaa2512.github.io/cintel-04-local/)

---

## Project Files

- `penguins/app.py` – Main PyShiny application
- `requirements.txt` – Required Python packages
- `.gitignore` – Git exclusion settings
- `README.md` – Project overview and instructions
- `docs/` – Static exported dashboard for GitHub Pages

---

##  Getting Started Locally

### 1. Clone the Repository

```bash
git clone https://github.com/Kiruthikaa2512/cintel-04-local.git
cd cintel-04-local
```

### 2. Create and Activate Virtual Environment

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

### 3. Install Required Packages

```bash
pip install -r requirements.txt
```

### 4. Run the App Locally

```bash
shiny run --reload --launch-browser penguins/app.py
```

> App opens in the browser at [http://127.0.0.1:8000](http://127.0.0.1:8000)

---

##  Static Export & GitHub Pages Deployment

### 5. Export to Static Files

```bash
.\.venv\Scripts\shinylive.exe export penguins docs
```

### 6. Preview Locally

```bash
py -m http.server --directory docs --bind localhost 8008
```

> Open [http://localhost:8008](http://localhost:8008) to test before publishing

### 7. Push Changes to GitHub

```bash
git add .
git commit -m "Exported static dashboard with bonus features"
git push
```

### 8. Enable GitHub Pages (One-Time Setup)

- Go to GitHub repo → **Settings → Pages**
- Source: `main` branch  
- Folder: `/docs`
- Save and wait for the published link to appear

---

##  Python Details

- Version: `Python 3.13.5`
- Verified with:
  ```bash
  python --version  # Python 3.13.5
  pip --version     # pip 24.x
  ```

- Python Installation Path (example):  
  `C:\Users\kirut\AppData\Local\Programs\Python\Python313\`

---

## Required Packages (via `requirements.txt`)

```text
faicons
palmerpenguins
pandas
pyarrow
plotly
seaborn
shiny
shinylive
shinywidgets
```

---

## App Features

- Plotly histogram, boxplot, scatterplot, and violin plots
- Seaborn histogram with KDE
- Reactive sidebar inputs to filter species, island, and selected attribute
-  Display of filtered DataFrame in table and grid formats
-  Download button for filtered data as CSV

---

## Bonus Features

-  **Reactive Summary Text**  
  Displays filter selection summary using species and island inputs

-  **Boxplot of Selected Attribute by Species**  
  Offers additional visual insight using Plotly

-  **Custom Tab Title**  
  Changed browser tab to “Penguin Explorer – Dashboard by Kiruthikaa”

---

##  Challenges Addressed

- Resolved `ModuleNotFoundError` by activating `.venv` and properly installing packages
- Adjusted CLI usage for `shinylive.exe` in PowerShell
- Fixed GitHub Pages build error by exporting correct `/docs` folder and committing it
- Verified deployment by visiting live dashboard and confirming reactive functionality

---

## Reflection

This project reflects hands-on experience with local development, Python-based interactivity, static export workflows, and cloud publishing using GitHub Pages. It demonstrates troubleshooting, customization, and bonus exploration — showcasing a complete deployment cycle using Python alone.

