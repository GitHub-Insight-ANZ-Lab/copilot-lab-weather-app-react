# Section 10: Deployment

## **Time:** 10 minutes


## Objectives:

*   Deploy the app to GitHub Pages or Netlify.
*   Understand Continuous Deployment considerations.


## Activities and GitHub Copilot Prompts:


### 10.1. Deploy to Netlify

1.  Create a Netlify Account
    *   Sign up at [Netlify](https://www.netlify.com/).

2.  Connect GitHub Repository
    *   Link your repository to Netlify.

3.  Configure Build Settings
    *   Set build command to `npm run build`.
    *   Publish directory is `build/`.


### 10.2. Use GitHub Actions for CI/CD

1.  Create a Workflow File
    *   In `.github/workflows/`, create `deploy.yml`.

2.  Type Workflow Configuration
    *   Type:
        ```yaml
        # GitHub Actions workflow for CI/CD
        ```
    *   Copilot Suggestion:
        ```yaml
        name: Build and Deploy

        on:
        push:
            branches:
            - main

        jobs:
        build:
            runs-on: ubuntu-latest
            steps:
            - uses: actions/checkout@v2
            - uses: actions/setup-node@v2
                with:
                node-version: '14'
            - run: npm install
            - run: npm run build
            - uses: actions/upload-artifact@v2
                with:
                name: build
                path: build
        ```
---------------
[Previous - Documentation and README Generation](08-documentation-and-readme-generation.md) | [Next - Conclusion and Next Steps](./10-conclusion.md)