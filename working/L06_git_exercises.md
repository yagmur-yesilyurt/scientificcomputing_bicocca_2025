# L06 Git - Exam Exercises
**Yagmur Yesilyurt**

## Q1: Version control for this course

I put my coursework under version control by forking the class repository
on GitHub:

- Remote repo: https://github.com/yagmur-yesilyurt/scientificcomputing_bicocca_2025
- All exercise solutions are committed to the `working/` directory
- I use `git add`, `git commit`, and `git push` to keep everything synced

This covers the full workflow: local edits -> staging -> commit -> push to remote.

## Q2: GitHub Action — commit guard

I wrote a GitHub Action (see `.github/workflows/check_readme.yml`) that runs
on every push and checks whether `README.md` contains my name.

If the name is missing the action fails with a non-zero exit code, which
blocks the commit from being considered "clean" in the CI pipeline.

To trigger it: push any change to the repo and check the Actions tab on GitHub.
