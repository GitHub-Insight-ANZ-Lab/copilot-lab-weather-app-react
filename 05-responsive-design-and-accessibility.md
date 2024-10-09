# Section 5: Responsive Design and Accessibility

**Time:** 15 minutes


## Objectives:

*   Implement basic responsive design with CSS.
*   Ensure basic accessibility compliance.


## Activities and GitHub Copilot Prompts:


### 5.1. Responsive Design with CSS

1.  Use Flexbox or Grid
    *   Open the **Chat View** and perform a **workspace** query like the following:
        ```
        @workspace Implement a responsive design that displays the forecast in a row on desktop but in a column on mobile
        ```
    *   Use follow-up queries to refine the suggestions, such as:
        ```
        I would like to use Grid layout
        ```
        or:
        ```
        Let's make the input and buttons fill the page width on mobile with a Flex layout
        ```
    *   Once you are happy with Copilot's suggestions, copy the code and style changes to their respective files


### 5.2. Accessibility Enhancements

1.  Add ARIA Labels
    *   Highlight the component markup and invoke the **Inline Chat** (`Ctrl+I` or `Cmd+I`)
    *   Prompt Copilot with a query such as the following:
        ```
        Add ARIA labels to make this accessible
        ```
    *   Copilot will suggest changes that you can apply by clicking Accept or using the hotkey (`Ctrl+Enter` or `Cmd+Enter`)
        
---------------
[Previous - State Management with React Hooks](./04-state-management-with-react-hooks.md) | [Next - Testing and Debugging](./06-testing.md)