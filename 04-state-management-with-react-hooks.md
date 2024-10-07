# Section 4: State Management with React Hooks

**Time:** 10 minutes


## Objectives:

*   Manage state using `useState` and `useEffect`.
*   Understand best practices for state management.


## Activities and GitHub Copilot Prompts:


### 4.1. Use `useEffect` to Fetch Data on Load

1.  Fetch Data When Component Mounts
    *   Type:
        ```tsx
        // Use useEffect to fetch data on component mount
        ```
    *   Copilot Suggestion:
        ```tsx
        useEffect(() => {
            fetchWeatherData("New York");
        }, []);
        ```


### 4.2. Handle Dependency Arrays

1.  Fetch Data When Units Change    
    *   Type:
        ```tsx
        // Re-fetch data when units change
        ```
    *   Copilot Suggestion:
        ```tsx
        useEffect(() => {
            if (city) {
                fetchWeatherData(city);
            }
        }, [units]);
        ```
        