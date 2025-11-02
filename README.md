# Jonas Pangerl — MkDocs Website

This repo contains my personal website built with **MkDocs Material** and hosted on **GitHub Pages**.
Use the commands below as a quick reference while working on the site.

---

## 0) Prerequisites

* Python 3.10+ recommended
* A virtual environment (venv)
* `mkdocs-material` installed
* Git + a GitHub repository (public)

### Create & activate venv

```bash
python -m venv .venv
# Windows:
.venv\Scripts\activate
# macOS / Linux:
source .venv/bin/activate
```

### Install dependencies

```bash
python -m pip install --upgrade pip
pip install mkdocs-material
# Optional extras (uncomment if used)
# pip install mkdocs-bootswatch
```

---

## 1) Local development

### Run local server (auto-reload on file changes)

```bash
mkdocs serve
```

* Opens at: [http://127.0.0.1:8000](http://127.0.0.1:8000)
* Stop with: `Ctrl+C`

### Build site locally (to check output)

```bash
mkdocs build
```

* Output is created in the `site/` folder.

### Clean build (remove previous output)

```bash
mkdocs build --clean
```


## 2) Git workflow

### First commit / routine commit & push

```bash
git add .
git commit -m "Update site content"
git push
```

### Set main branch (first time only)

```bash
git branch -M main
git push -u origin main
```

---

## 3) Publish to GitHub Pages

**MkDocs will build and push to the `gh-pages` branch automatically.**

```bash
mkdocs gh-deploy --force
```

* Live URL: `https://<YOUR-GITHUB-USER>.github.io/<REPO>/`
* If the page doesn’t appear, check **GitHub → Repo → Settings → Pages**

  * Source: **Deploy from a branch**
  * Branch: **gh-pages** / **/** (root)

