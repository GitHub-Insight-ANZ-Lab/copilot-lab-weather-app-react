# Section 1: Project Initialization

**Time:** 10 minutes

## Objectives

- Set up a new React and TypeScript project
- Configure Git and GitHub Copilot
- Initialise the project repository

## Activities and GitHub Copilot Prompts

### 1.1. Create a New React and TypeScript Project

1. Initialise Project with Create React App

   ```bash
   npm create vite@latest weather-app -- --template react-ts
   ```

2. Navigate to Project Directory

   ```bash
   cd weather-app
   ```

3. Start the Development Server

   ```bash
   npm run start
   ```

### 1.2. Set Up GitHub Copilot

1. Install GitHub Copilot Extension in VSCode

   - Go to Extensions (`Ctrl+Shift+X` or `Cmd+Shift+X`)
   - Search for "GitHub Copilot" and install it

2. Sign In to GitHub

   - Follow the prompts to authenticate

3. Test GitHub Copilot

   - Open `src/App.tsx`
   - Invoke the **Inline Chat** (`Ctrl+I` or `Cmd+I`)
   - Prompt Copilot with a request like the following:

     ```md
     Create a functional component that displays "Hello, World!"
     ```

   - It should respond with a suggestion such as:

     ```tsx
     const HelloWorld = () => {
       return <p>Hello, World!</p>;
     };
     ```

4. Accept the Suggestion
   - Click `Accept` or use the hotkey (`Ctrl+Enter` or `Cmd+Enter`) to accept Copilot's suggestion

---

[Previous - Home](./README.md) | [Next - Building the weather app core](./02-building-the-weather-app-core.md)
