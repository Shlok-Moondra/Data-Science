# Data Science Learning Notebooks

> A structured Jupyter Notebook workspace for learning Data Science fundamentals first, then gradually moving toward Machine Learning and industry-style project workflows.

## Overview

This repository is my hands-on learning space for Data Science. The current priority is to build strong fundamentals before moving into advanced Machine Learning topics.

The notebooks are used to practice:

- Python for data analysis
- Jupyter Notebook workflows
- Pandas basics and data manipulation
- Exploratory Data Analysis concepts
- Clean, repeatable notebook habits
- Version control for learning projects

## Repository Structure

```text
juypter/
+-- numpy1.ipynb
+-- pandas.ipynb
+-- numpy2.ipynb
+-- venv/
`-- README.md
```

## Learning Roadmap

The learning path in this folder starts with Data Science first:

1. Python basics for analysis
2. Jupyter Notebook usage
3. NumPy fundamentals
4. Pandas for data cleaning and transformation
5. Data visualization with Matplotlib and Seaborn
6. Exploratory Data Analysis
7. Statistics for Data Science
8. Feature engineering
9. Introductory Machine Learning
10. Model evaluation and project documentation

## Prerequisites

Install these tools before running the notebooks:

- Python 3.10 or newer
- Git
- Visual Studio Code or JupyterLab
- pip, Python's package manager

Check your installed versions:

```bash
python --version
pip --version
git --version
```

On Windows, if `python` does not work, try:

```bash
py --version
```

## Getting Started

Clone the repository:

```bash
git clone <repository-url>
cd juypter
```

If you already have the folder locally, move into it:

```bash
cd "D:\Machine learning\juypter"
```

## Virtual Environment Setup

Create a virtual environment:

```bash
python -m venv venv
```

Activate it on Windows PowerShell:

```bash
.\venv\Scripts\Activate.ps1
```

Activate it on Windows Command Prompt:

```bash
venv\Scripts\activate.bat
```

Activate it on macOS or Linux:

```bash
source venv/bin/activate
```

Upgrade pip:

```bash
python -m pip install --upgrade pip
```

Install common Data Science packages:

```bash
pip install jupyter jupyterlab notebook numpy pandas matplotlib seaborn scipy scikit-learn
```

Optional packages that are useful later:

```bash
pip install plotly openpyxl statsmodels
```

## Running the Notebooks

Start Jupyter Notebook:

```bash
jupyter notebook
```

Or start JupyterLab:

```bash
jupyter lab
```

Then open one of the notebooks:

- `numpy1.ipynb`
- `pandas.ipynb`
- `numpy2.ipynb`

## VS Code Workflow

Open the folder in VS Code:

```bash
code .
```

Select the notebook kernel:

1. Open any `.ipynb` file.
2. Click the kernel selector in the top right.
3. Choose the Python interpreter from `venv`.
4. Run cells one by one.

If the virtual environment does not appear as a kernel, install and register it:

```bash
pip install ipykernel
python -m ipykernel install --user --name juypter-venv --display-name "Python (juypter-venv)"
```

## Dependency Management

Save installed packages:

```bash
pip freeze > requirements.txt
```

Install packages from `requirements.txt`:

```bash
pip install -r requirements.txt
```

Check outdated packages:

```bash
pip list --outdated
```

Show installed packages:

```bash
pip list
```

## Recommended Git Workflow

Check current changes:

```bash
git status
```

Add changed files:

```bash
git add .
```

Commit changes:

```bash
git commit -m "Add data science learning notebooks"
```

View commit history:

```bash
git log --oneline
```

Push changes:

```bash
git push origin main
```

If your branch is named `master`, use:

```bash
git push origin master
```

## Notebook Best Practices

- Keep notebooks focused on one topic at a time.
- Restart the kernel and run all cells before committing.
- Add markdown explanations between important code blocks.
- Use clear variable names.
- Keep raw data separate from processed data when datasets are added.
- Avoid committing large generated files.
- Do not commit virtual environments, cache files, or notebook checkpoints.

## Suggested `.gitignore`

Use a `.gitignore` file to keep the repository clean:

```gitignore
venv/
.venv/
__pycache__/
*.pyc
.ipynb_checkpoints/
.env
.DS_Store
```

## Common Troubleshooting

If script execution is blocked in PowerShell:

```bash
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

If Jupyter is not recognized:

```bash
pip install jupyter
python -m jupyter notebook
```

If a package is missing:

```bash
pip install package-name
```

If the notebook kernel is using the wrong Python version:

```bash
where python
python -m ipykernel install --user --name juypter-venv --display-name "Python (juypter-venv)"
```

## Project Status

This is an active learning repository. The current focus is Data Science foundations, especially Python, Pandas, notebooks, and practical analysis habits. Machine Learning topics will be added after the Data Science base becomes stronger.

## Author

Maintained by Shlok as part of a personal Data Science learning journey.
