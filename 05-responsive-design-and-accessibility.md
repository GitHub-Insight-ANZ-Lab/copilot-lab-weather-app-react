# Section 5: Responsive Design and Accessibility

**Time:** 15 minutes


## Objectives:

*   Implement responsive design with CSS.
*   Ensure accessibility compliance.


## Activities and GitHub Copilot Prompts:


### 5.1. Responsive Design with CSS

1.  Use Flexbox or Grid
    *   Type in `App.css`:
        ```css
        /* Make the main content responsive */
        ```
    *   Copilot Suggestion:
        ```css
        main {
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 20px;
        }
        ```
        
2.  Add Media Queries
    
    *   Type:
        ```css
        /* Adjust layout for smaller screens */
        ```
    *   Copilot Suggestion:
        ```css
        @media (max-width: 600px) {
            .weather-container {
                flex-direction: column;
            }
        }
        ```


### 5.2. Accessibility Enhancements

1.  Add ARIA Labels
    *   In input fields:
        ```tsx
        <input
            type="text"
            aria-label="City"
            ...
        />
        ```

2.  Ensure Keyboard Navigation
    *   Type:
        ```tsx
        // Make the get current location button focusable
        ```
    *   Copilot Suggestion:
        ```tsx
        <button
            onClick={getCurrentLocation}
            tabIndex={0}
        >
            Use Current Location
        </button>
        ```
        
---------------
[Previous - State Management with React Hooks](./04-state-management-with-react-hooks.md) | [Next - Performance Optimisation](./06-performance-optimisation.md)