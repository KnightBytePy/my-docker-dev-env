# ML Dev Container Template 🐳

Reusable Docker + VS Code Dev Container setup for Python / Data Science / ML.

Use this repo as a base for any project so you get a consistent environment on
Windows / macOS / Linux with:

- Python 3.11
- Common DS/ML stack (NumPy, pandas, scikit-learn, PyTorch, XGBoost, etc.)
- Jupyter + VS Code + useful extensions
- Reproducible dependencies via `requirements.txt`

---

## 🔧 How to use this template

### 1. Use this repo as a template

You have two options:

1. **Template for new projects**

   - On GitHub, click **Use this template** → **Create a new repository**
   - Name it after your project (e.g. `customer-churn-streamlit-xgboost`)
   - Clone that new repo locally
   - Open it in VS Code → follow **“Open in Dev Container”** below

2. **Just use this repo as a generic dev env**

   - Clone this repo directly and work inside it for experiments / notebooks.

---

## 🧰 Requirements

- [Docker Desktop](https://www.docker.com/products/docker-desktop) installed and running
- [VS Code](https://code.visualstudio.com/)
- VS Code extension: **Dev Containers** (ms-vscode-remote.remote-containers)

---

## ▶️ Open in VS Code Dev Container

1. Open this folder in VS Code.
2. Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on macOS).
3. Run: **Dev Containers: Reopen in Container**.

VS Code will:

- Build the Docker image from `Dockerfile`.
- Start a container.
- Attach VS Code to it.

Then you can:

- Run notebooks in the container (Python kernel).
- Run scripts / apps with the same environment everywhere.

---

## 🐳 Using Docker directly

Build the image:

```bash
docker build -t ml-dev-env .
