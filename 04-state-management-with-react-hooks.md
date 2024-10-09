# Section 4: State Management with React Hooks

**Time:** 10 minutes

## Objectives

- Fetch and update data using `useEffect`.

## Activities and GitHub Copilot Prompts

### 4.1. Use `useEffect` to Fetch Data on Load

1. Fetch Data When Component Mounts

   - Open the **Chat View** and perform the following **workspace** query:

     ```md
     @workspace Use useEffect to fetch data on component mount
     ```

   - Copilot should suggest how you can add a `useEffect` hook to fetch data when the `App` component first mounts

### 4.2. Handle Dependency Arrays

1. Fetch Data When Units Change

   - As a follow-up, tell Copilot the following:

     ```md
     I would also like to re-fetch the data when units change
     ```

   - Copilot will tell you how to modify the `useEffect` so that it will re-fetch the data if you change the units

---

[Previous - Implementing Advanced Features](./03-implementing-advanced-features.md) | [Next - Responsive Design and Accessibility](./05-responsive-design-and-accessibility.md)
