# Section 1: Project Initialization

**Time:** 10 minutes


## Objectives:

*   Set up a new React and TypeScript project
*   Configure Git and GitHub Copilot
*   Initialise the project repository


## Activities and GitHub Copilot Prompts:


### 1.1. Create a New React and TypeScript Project

1.  Initialise Project with Create React App
    ```bash
    npx create-react-app weather-app --template typescript
    ```

2.  Navigate to Project Directory
    ```bash
    cd weather-app
    ```

3.  Start the Development Server
    ```bash
    npm start
    ```


### 1.2. Initialise Git Repository

1.  Initialise Git
    ```bash
    git init
    ```
    
2.  Add All Files
    ```bash
    git add .
    ```
    
3.  Commit Changes
    ```bash
    git commit -m "Initial commit"
    ```
    

### 1.3. Set Up GitHub Copilot

1.  Install GitHub Copilot Extension in VSCode
    *   Go to Extensions (`Ctrl+Shift+X` or `Cmd+Shift+X`)
    *   Search for "GitHub Copilot" and install it

2.  Sign In to GitHub
    *   Follow the prompts to authenticate

3.  Test GitHub Copilot
    *   Open `src/App.tsx`
    *   Invoke the **Inline Chat** (`Ctrl+I` or `Cmd+I`)
    *   Prompt Copilot with a request like the following:
        ```
        Create a functional component that displays "Hello, World!"
        ```
    *   It should respond with a suggestion such as:
        ```tsx
        const HelloWorld = () => {
            return <p>Hello, World!</p>;
        };
        ```
        
4.  Accept the Suggestion
    *   Click `Accept` or use the hotkey (`Ctrl+Enter` or `Cmd+Enter`) to accept Copilot's suggestion
