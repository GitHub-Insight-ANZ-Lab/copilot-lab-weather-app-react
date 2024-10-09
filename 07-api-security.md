# Section 8: API Security

**Time:** 10 minutes


## Objectives:

*   Protect API keys.
*   Use environment variables securely.


## Activities and GitHub Copilot Prompts:


### 8.1. Ensure `.env` is in `.gitignore`

1.  Check `.gitignore`
    *   Type:
        ```gitignore
        # Ignore environment variables
        ```
    *   Copilot Suggestion:
        ```gitignore
        .env
        ```


### 8.2. Use HTTPS and Handle CORS

1.  Ensure API Calls Use HTTPS
    *   Verify that API URLs start with `https://`.

2.  Handle CORS Errors
    *   Discuss using proxy servers or configuring headers if needed.

---------------
[Previous - Testing and Debugging](./06-testing-and-debugging.md) | [Next - Documentaion and readme generation](./08-documentation-and-readme-generation.md)