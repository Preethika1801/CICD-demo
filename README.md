
 🚀 CICD-demo: GitHub Actions CI/CD Example

## 1) What is this Project?

**CICD-demo** is a lightweight project that demonstrates how to set up **Continuous Integration (CI)** and **Continuous Deployment (CD)** using **GitHub Actions**.

This setup helps automate testing and deployment tasks, reducing manual work and increasing reliability.

## 2) Why CI/CD?

Using CI/CD brings major benefits to modern software projects:

- ✅ **Automated Testing**: Ensures code is validated before merging.
- 🚀 **Faster Deployment**: Push changes, and see them in action automatically.
- 🛡️ **Better Code Quality**: Bugs are caught early through tests.
- 🔄 **Speedy Development**: Reduces release time and manual steps.

## 3) What’s in the Project?

- A basic Python script.
- A test file to validate the code.
- A GitHub Actions workflow that runs tests automatically when changes are pushed or pull requests are created.

| File/Folder               | Purpose                                     |
|--------------------------|---------------------------------------------|
| `app.py`                 | Main Python script.                         |
| `test_app.py`            | A simple unit test.                         |
| `req.txt`                | Dependency list.                            |
| `.github/workflows/`     | Contains the CI/CD workflow YAML file.      |

## 4) How to Access and Run the Project

### 📥 Clone the Repo:

```bash
git clone https://github.com/Preethika1801/CICD-demo.git
cd CICD-demo
```

### 💻 Run Locally on VS Code:

1. Open the folder in VS Code.
2. Make sure Python is installed.
3. Install requirements:
   ```bash
   pip install -r req.txt
   ```
4. Run the app:
   ```bash
   python app.py
   ```
5. Run tests:
   ```bash
   pytest test_app.py
   ```

## 5) How GitHub Actions Work in This Project

Once you push code to the repository or create a pull request, GitHub Actions will:

- Set up a Python environment.
- Install dependencies from `req.txt`.
- Run the test file using `pytest`.

The `.github/workflows/main.yml` file contains the full CI/CD logic.

## 6) How to Test the Pipeline Yourself

You can test the GitHub Actions pipeline easily:

### Option 1: Test on VS Code

- Make a code change in `test_app.py` (e.g., add `print("Hello CI")`).
- Run the tests locally with `pytest` to see if it works.

### Option 2: Upload to Your GitHub

1. Fork or create a new GitHub repo.
2. Push this project to your repo:
   ```bash
   git remote add origin <your-repo-url>
   git push -u origin main
   ```
3. Make a change (like updating a print statement) and push it.
4. Go to the **Actions** tab on your GitHub repo.
5. Watch the CI pipeline run and check if it passes or fails.

🧠 Note:
To ensure the test passes and the GitHub Actions workflow runs successfully, the print statement in app.py should exactly match what is being checked in test_app.py.

If there's any mismatch, the test will fail, and you'll see an error in the Actions tab during the CI/CD process.

## 7) Check Workflow Results

- Visit the **Actions tab** in your GitHub repo.
- Review logs for each CI job step.
- If something fails, GitHub will show exactly where and why.

## 8) 📌 Summary

✅ Clone or fork the repo  
✅ Make changes locally or in GitHub  
✅ GitHub Actions automatically runs your tests  
✅ See pass/fail feedback in the Actions tab  
✅ Improve and iterate faster with confidence!
