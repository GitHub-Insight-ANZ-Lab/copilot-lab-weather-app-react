# Section 7: Testing and Debugging

**Time:** 10 minutes


## Objectives:

*   Write tests with Jest and React Testing Library.
*   Use GitHub Copilot to generate test cases.


## Activities and GitHub Copilot Prompts:


### 7.1. Write a Simple Test

1.  Create a Test File
    *   Create `App.test.tsx`.

2.  Type Test Description
    *   Type:
        ```tsx
        // Test if the App component renders without crashing
        ```
    *   Copilot Suggestion:
        ```tsx
        test("renders App component without crashing", () => {
            const div = document.createElement("div");
            ReactDOM.render(<App />, div);
            ReactDOM.unmountComponentAtNode(div);
        });
        ```


### 7.2. Test Event Handlers

1.  Type Test for Fetch Function
    *   Type:
        ```tsx
        // Test fetchWeatherData function with a mock API call
        ```
    *   Copilot Suggestion:
        ```tsx
        test("fetchWeatherData fetches data successfully", async () => {
            // Mock API call and test
        });
        ```


### 7.3. Debugging Tips

1.  Use VSCode Debugger
    *   Set breakpoints and inspect variables.

2.  Console Logging
    *   Type:
        ```tsx
        // Log weather data for debugging
        ```
    *   Copilot Suggestion:
        ```tsx
        console.log(weatherData);
        ```

---------------
[Previous - Responsive Design and Accessibility](./05-responsive-design-and-accessibility.md) | [Next - API security](./07-api-security.md)