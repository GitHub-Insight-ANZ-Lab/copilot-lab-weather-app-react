# Section 13: Git Workflows and Collaboration

## **Time:** 10 minutes


## Objectives:

*   Understand Git branching strategies.
*   Use pull requests and code reviews.
*   Integrate GitHub Copilot into collaborative workflows.


## Activities and GitHub Copilot Prompts:


### 11.1. Create a New Branch

1.  Create Feature Branch
    ```bash
    git checkout -b feature/add-dark-mode
    ```

2.  Implement Feature
    *   Use Copilot to assist in adding a dark mode toggle.


### 11.2. Push Branch and Create Pull Request

1.  Push Branch to GitHub
    ```bash
    git push origin feature/add-dark-mode
    ```

2.  Create Pull Request
    *   On GitHub, open a pull request for the new feature.


### 11.3. Code Review

1.  Review Changes
    *   Use GitHub's code review tools.

2.  Merge Pull Request
    *   After approval, merge the feature branch into `main`.


### 11.4. Use Copilot for Commit Messages

1.  Stage Changes
    ```bash
    git add .
    ```

2.  Type Commit Message
    *   Type:
        ```bash
        git commit -m "
        ```
    *   Copilot Suggestion:
        ```bash
        git commit -m "Add dark mode toggle feature"
        ```

---------------
[Previous - Deployment](./10-deployment.md) | [Next - Conclusion and Next Steps](./12-conclusion.md)