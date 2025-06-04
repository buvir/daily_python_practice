# Daily_python_practice


A collection of solved Python problems and tutorials, including regular expressions, pandas, API usage, and intermediate Python exercises. This repository is designed as a study resource for learning and practicing Python programming.

---

## 📁 Project Structure

- **API.ipynb**: Examples and exercises on APIs, including fetching weather data and deploying ML models with Flask.
- **EDA_Tutorial_python.ipynb**: Exploratory Data Analysis tutorials using Python (likely with pandas, matplotlib, etc.).
- **Pandas_Tutorial_my.ipynb**: Hands-on pandas exercises and explanations.
- **Python_Intermediate_Solutions.ipynb**: Solutions to intermediate-level Python problems.
- **Regex_Solutions.ipynb**: Regex problem solutions (HackerRank and custom).
- **Regex_Tutorial.ipynb**: In-depth regular expressions tutorial with examples and explanations.
- **README.md**: This file.

## 📊 filter_method.ipynb — Feature Selection with Filter Methods

This notebook demonstrates **filter methods** for feature selection in machine learning using Python. Filter methods evaluate the relevance of features by their statistical relationship with the target variable, independent of any machine learning model.

### Key Steps Covered

- **Correlation Analysis:**  
  - Calculates the correlation between features (like `age`, `income`) and the target (`loan_approval`) to identify the most relevant features.
- **SelectKBest with ANOVA F-test:**  
  - Uses `SelectKBest` from `sklearn.feature_selection` with the `f_classif` score function to select the top features for classification tasks (demonstrated on the Iris dataset).

### Libraries Used

- `pandas` — Data manipulation and analysis  
  [pandas documentation](https://pandas.pydata.org/docs/)
- `scikit-learn` — Feature selection utilities  
  [scikit-learn documentation](https://scikit-learn.org/stable/documentation.html)

### Example Datasets

- **Loan Approval Example:**  
  Small synthetic dataset with `age`, `income`, and `loan_approval` columns.
- **Iris Dataset:**  
  Classic multiclass classification dataset included in scikit-learn.

### Why Use Filter Methods?

Filter methods are fast and model-agnostic, making them suitable for quickly reducing the number of features before applying more complex selection or modeling techniques.



---

## 🐍 Setting Up a Python Virtual Environment (venv) in CodeSpaces

A virtual environment keeps your project dependencies isolated.

**Create a virtual environment:**
```bash
python -m venv .venv
```

**Activate the virtual environment:**
```bash
source .venv/bin/activate
```

**Deactivate the virtual environment:**
```bash
deactivate
```

**Install dependencies:**
```bash
pip install -r requirements.txt
```
*(Create `requirements.txt` with your needed packages, e.g., `pip freeze > requirements.txt`)*

**More on venv:**  
- [Python venv documentation](https://docs.python.org/3/library/venv.html)
- [Real Python: Python Virtual Environments](https://realpython.com/python-virtual-environments-a-primer/)

---

## 📚 Libraries Used & Documentation

| Library      | Usage Example(s)                | Documentation Link                                         |
|--------------|---------------------------------|------------------------------------------------------------|
| `re`         | Regular expressions             | https://docs.python.org/3/library/re.html                  |
| `pandas`     | Data analysis, EDA              | https://pandas.pydata.org/docs/                            |
| `requests`   | API calls (HTTP requests)        | https://docs.python-requests.org/en/latest/                |
| `flask`      | Simple web API (ML deployment)   | https://flask.palletsprojects.com/en/latest/               |
| `pickle`     | Model serialization             | https://docs.python.org/3/library/pickle.html              |
| `sklearn`    | Machine learning models          | https://scikit-learn.org/stable/documentation.html         |
| `string`     | String constants (punctuation)   | https://docs.python.org/3/library/string.html              |
| `collections`| Data structures (defaultdict)    | https://docs.python.org/3/library/collections.html         |

*(Not all libraries may be used in every notebook; check each notebook for imports.)*

---

## 📝 Key Python/Regex Definitions

- **Regular Expression (Regex):** A sequence of characters that forms a search pattern, mainly for string matching and manipulation.
- **pandas:** A Python library for data manipulation and analysis, providing DataFrame and Series objects.
- **requests:** A simple HTTP library for Python, used to send HTTP requests and interact with APIs.
- **Flask:** A lightweight web framework for building APIs and web applications in Python.
- **pickle:** A module for serializing and deserializing Python objects.
- **venv:** A built-in Python module to create isolated virtual environments.
- **defaultdict:** A subclass of dict that returns a default value if the key is missing.

---

## 🚀 GitHub Repository Workflow Checklist

### 1. Verify It’s Your Repository
```bash
git remote -v  # Check if URL has YOUR username (github.com/your-username/repo-name)
gh auth status  # Confirm logged-in GitHub account (requires GitHub CLI)
```

### 2. Sync with Remote (Pull Latest Changes)
```bash
git pull origin main  # Pull latest changes (replace "main" with your branch)
```

### 3. Stage and Commit Changes
```bash
git add .                        # Stage all changes
git commit -m "Your message"     # Commit changes
```

### 4. Push to Origin (Normal Push)
```bash
git push origin main             # Push to main branch
```

### 5. Force Push (Only if Necessary!)
```bash
git push --force origin main     # Overwrites remote history (use with caution!)
```

### 6. Rebase and Force Push (Advanced)
```bash
git pull --rebase origin main    # Rebase local changes on top of remote
git push --force-with-lease      # Safer force push (checks for new remote commits)
```

### 7. Resolve Common Errors

**"Updates were rejected" (Remote has new changes):**
```bash
git pull origin main           # Pull latest changes first
git push origin main           # Try pushing again
```

**Merge conflicts:**  
Open conflicted files, resolve conflicts (look for `<<<<<<< HEAD` markers).

After fixing:
```bash
git add .                      # Mark conflicts as resolved
git commit -m "Resolved merge conflicts"
git push origin main
```

**"Permission denied":**
```bash
gh auth login                  # Re-authenticate with GitHub CLI
git remote set-url origin git@github.com:your-username/repo-name.git  # Ensure correct remote
```

### 8. Reset and Revert

**Undo last commit (local only):**
```bash
git reset --soft HEAD~1        # Keeps changes staged
```

**Undo pushed commit:**
```bash
git revert <commit-hash>       # Creates a new undo commit
git push origin main
```

---

## 📝 How to Use This README as Study Material

- Refer to the **project structure** to find relevant notebooks for each topic.
- Use the **library table** to quickly find documentation and understand what each library is used for.
- Follow the **virtual environment setup** to keep your dependencies isolated and reproducible.
- Use the **GitHub workflow checklist** for smooth version control and collaboration.
- Review the **definitions** section to reinforce your Python and regex fundamentals.

---

## 🔗 Additional Resources

- [Python Official Documentation](https://docs.python.org/3/)
- [GitHub Docs: Working with Codespaces](https://docs.github.com/en/codespaces)
- [HackerRank Regex Practice](https://www.hackerrank.com/domains/tutorials/10-days-of-javascript?filters%5Bsubdomains%5D%5B%5D=regex)

---

Happy coding and learning!
