![image](https://github.com/user-attachments/assets/36ce1d81-cabb-402a-93ea-f58501877de4)

![image](https://github.com/user-attachments/assets/136a958e-7d63-4047-8d32-c5d11870b6ec)

![Uploading image.png…]()


Assignment 4 
Husky is a popular tool used in Git projects to automate quality checks and enforce rules before code is committed or pushed. It integrates with Git hooks (scripts triggered at certain points in the Git lifecycle, like before a commit) and allows developers to run commands such as code linters, formatters, or commit message validators automatically. This helps teams maintain consistent code style, avoid errors, and follow best practices without relying solely on manual reviews

Git Workflow with Husky

On running git commit, Husky triggers the pre-commit hook, running tools like ESLint and Prettier via lint-staged.

If any issues are found , the commit is blocked until fixed.

On committing with a message, Husky's commit-msg hook runs commitlint, checking the format .

After a successful commit and push to GitHub, GitHub Actions runs a CI workflow, automatically performing additional checks like linting or tests.

The workflow passes or fails visibly in the GitHub interface, giving feedback to the developer or reviewer.
