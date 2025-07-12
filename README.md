````markdown
# cintel-04-local

This repository contains the local development version of a PyShiny dashboard project. It supports local development using Python, Visual Studio Code, and Git.

## Project Files

- `app.py` – Main PyShiny application
- `requirements.txt` – List of required Python packages
- `.gitignore` – Tells Git which files to ignore
- `README.md` – Project overview and setup instructions

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/cintel-04-local.git
cd cintel-04-local
````

### 2. Create and Activate a Virtual Environment

```powershell
python -m venv venv
.\venv\Scripts\Activate.ps1
```

### 3. Install Required Packages

```bash
pip install -r requirements.txt
```

### 4. Run the Shiny App

```bash
python app.py
```

## Python Version

This project uses **Python 3.13.5**.

### Verified With

```powershell
python --version
# Python 3.13.5

pip --version
# pip 24.x from ... (python 3.13)
```

### Python Installation Path (Example)

```
C:\Users\kirut\AppData\Local\Programs\Python\Python313\
```

## Required Packages

Listed in `requirements.txt`:

```
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

