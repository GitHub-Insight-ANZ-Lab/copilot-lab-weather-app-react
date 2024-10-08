# Section 2: Building the Weather App Core

**Time:** 25 minutes


## Objectives:

*   Set up the basic layout with CSS.
*   Integrate OpenWeatherMap API.
*   Utilize GitHub Copilot for API calls.


## Activities and GitHub Copilot Prompts:


### 2.1. Set Up Basic Layout

1.  Create a Basic Layout
    *   Open the Copilot **Chat View** (`Ctrl+Alt+I` or `Cmd+Alt+I`)
    *   Prompt Copilot with a **workspace** query like the following:
        ```
        @workspace Create a basic layout with a header and main section
        ```
    *   This should provide suggestions for both the React component, as well as the associated styles
    *   Copy the component code into `App.tsx`
        
2.  Apply Basic Styles
    *   Copy the component styles into `App.css`


### 2.2. Integrate OpenWeatherMap API

1.  Obtain API Key
    *   Sign up at [OpenWeatherMap](https://openweathermap.org/price) to get a Free API key

2.  Store API Key in Environment Variable
    *   Create a new file in the project root called `.env`
    *   Add the API key:
        ```env
        REACT_APP_WEATHER_API_KEY=your_api_key_here
        ```
        
3.  Fetch Weather Data
    *   In `App.tsx`, type the following:
        ```tsx
        // Function to fetch weather data for a city
        ```
    *   Copilot will generate an **inline suggestion** from your code comment
    *   You can cycle through several suggestions by clicking the previous/next arrows, or by using the hotkeys (`Alt+[`/`Alt+]`)
    *   Press `Tab` to accept the suggested code
        
4.  Handle User Input
    *   Add a state variables for the city and weather to your `App` component:
        ```tsx
        const [city, setCity] = useState<string>("");
        const [weather, setWeather] = useState<any>();
        ```
    *   Now try using **inline suggestions** to add an input field for the city, as well as a button to fetch the current weather

5.  Display Weather Data
    *   Open the **Chat View** and ask a **workspace** question like the following:
        ```
        @workspace If weather data is available, display the city name and current temperate
        ```
    *   Copy the relevant code into your `App` component where applicable and try running the app
    *   You may find that the app has encountered an error, or does not work in the way you expected. Because this is a chat interaction, you can ask follow-up questions to refine the output.

---------------
[Previous - Project initialisation](./01-project-initialisation.md) | [Next - Implementing advanced features](./03-implementing-advanced-features.md)