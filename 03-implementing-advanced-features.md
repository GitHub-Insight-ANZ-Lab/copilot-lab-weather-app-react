# Section 3: Implementing Advanced Features

**Time:** 20 minutes

## Objectives

- Add 5-day forecast functionality.
- Implement unit switching.

## Activities and GitHub Copilot Prompts

### 3.1. Add 5-Day Forecast

1. Fetch Forecast Data

   - In the `App` component, add a new state variable for forecast data

     ```tsx
     const [forecast, setForecast] = useState<any>();
     ```

   - Try prompting Copilot for the following:

     ```md
     Function to fetch the 5-day weather forecast for a city
     ```

   - Highlight the existing `onClick` code and invoke the **Inline Chat** (`Ctrl+I` or `Cmd+I`) and try prompting it with the following:

     ```md
     Fetch weather and forecast data, then set the respective states
     ```

   - Copilot should provide a new implementation of the `onClick` behaviour

2. Display Forecast Data

   - Below the city weather display, invoke the **Inline Chat** again and prompt it with the following:

     ```md
     Map over forecast data to display it
     ```

### 3.2. Implement Unit Switching

1. Add State for Units

   ```tsx
   const [units, setUnits] = useState<string>("metric");
   ```

2. Create a Toggle Button

   - Move the cursor below the Get Weather button, invoke the **Inline Chat** and prompt Copilot for the following:

     ```md
     Button to switch units
     ```

3. Update Fetch Functions

   - Highlight the fetch functions, invoke the **Inline Chat** and prompt Copilot to do the following:

     ```md
     Modify the API calls to include units
     ```

4. Update the Units Displayed

   - Highlight the temperature markup, invoke the **Inline Chat** and prompt Copilot to do the following:

     ```md
     Display the correct unit abbreviation
     ```

---

[Previous - Building the weather app core](./02-building-the-weather-app-core.md) | [Next - State management with react hooks](./04-state-management-with-react-hooks.md)
