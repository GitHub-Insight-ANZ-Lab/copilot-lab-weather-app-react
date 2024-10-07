# Section 6: Performance Optimisation

**Time:** 10 minutes


## Objectives:

*   Identify performance bottlenecks.
*   Use React's memoisation techniques.


## Activities and GitHub Copilot Prompts:


### 6.1. Use `React.memo`

1.  Optimise Components
    *   Type:
        ```tsx
        // Wrap the Forecast component with React.memo
        ```
    *   Copilot Suggestion:
        ```tsx
        export default React.memo(Forecast);
        ```


### 6.2. Use `useMemo` and `useCallback`

1.  Memoise Computed Values
    *   Type:
        ```tsx
        // Memoise the formatted weather data
        ```
    *   Copilot Suggestion:
        ```tsx
        const formattedWeatherData = useMemo(() => {
            // Format data here
        }, [weatherData]);
        ```

2.  Optimise Event Handlers
    *   Type:
        ```tsx
        // Use useCallback for the handleSearch function
        ```
    *   Copilot Suggestion:
        ```tsx
        const handleSearch = useCallback(() => {
            fetchWeatherData(city);
        }, [city, units]);
        ```
