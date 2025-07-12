````markdown
# cintel-04-local

This repository contains the local development version of our PyShiny dashboard project. We are transitioning from using Shiny in the browser to running and developing apps locally using Python, VS Code, and Git.

## Project Structure

- `app.py` – Main Shiny application file.
- `requirements.txt` – List of required Python packages.
- `.gitignore` – Tells Git which files/folders to ignore (e.g., venv/).
- `README.md` – This file.

## Setup Instructions

### 1. Clone the Repository

```bash
git clone [https://github.com/YOUR_USERNAME/cintel-04-local.git](https://github.com/Kiruthikaa2512/cintel-04-local)
````

### 2. Create and Activate a Virtual Environment

```bash
python -m venv venv
.\venv\Scripts\Activate.ps1    # For PowerShell
```

### 3. Install Requirements

```bash
pip install -r requirements.txt
```

### 4. Run the App

```bash
python app.py
```

## Python Version

This project uses Python 3.13.5.

### Verified Using:

```powershell
python --version
# Output: Python 3.13.5

pip --version
# Output: pip 24.x from ... (python 3.13)
```

### Python Install Location

On my system, Python is installed at:

```
C:\Users\kirut\AppData\Local\Programs\Python\Python313\
```

## Packages Used

These packages are listed in `requirements.txt`:

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
