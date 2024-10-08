# Section 3: Implementing Advanced Features

**Time:** 20 minutes


## Objectives:

*   Add 5-day forecast functionality.
*   Implement unit switching.
*   Enable location search.


## Activities and GitHub Copilot Prompts:


### 3.1. Add 5-Day Forecast

1.  Update Fetch Function
    *   Type:
        ```tsx
        // Function to fetch 5-day forecast data`
        ```
    *   Start typing:
        ```tsx
        const fetchForecastData = async (city: string) => {
        ```
    *   Copilot Suggestion:
        ```tsx
            const response = await fetch(
                `https://api.openweathermap.org/data/2.5/forecast?q=${city}&appid=${process.env.REACT_APP_WEATHER_API_KEY}&units=metric`
            );
            const data = await response.json();
            setForecastData(data);
        };
        ```
        
2.  Display Forecast Data
    *   Type:
        ```tsx
        // Map over forecast data to display it
        ```
    *   Copilot Suggestion:
        ```tsx
        {forecastData.list.map((item) => (
            <div key={item.dt}>
                <p>{new Date(item.dt_txt).toLocaleString()}</p>
                <p>{item.main.temp}°C</p>
            </div>
        ))}
        ```


### 3.2. Implement Unit Switching

1.  Add State for Units
    ```tsx
    const [units, setUnits] = useState<string>("metric");
    ```

2.  Create a Toggle Button
    *   Type:
        ```tsx
        // Button to switch units
        ```
    *   Copilot Suggestion:
        ```tsx
        <button onClick={() => setUnits(units === "metric" ? "imperial" : "metric")}>
            Switch to {units === "metric" ? "Imperial" : "Metric"}
        </button>
        ```
        
3.  Update Fetch Functions
    *   Modify API calls to include `units`:
        ```tsx
        `...&units=${units}`
        ```

### 3.3. Enhance Location Search

1.  Use Geolocation API
    *   Type:
        ```tsx
        // Function to get user's current location
        ```
    *   Start typing:
        ```tsx
        const getCurrentLocation = () => {
        ```
    *   Copilot Suggestion:
        ```tsx
            navigator.geolocation.getCurrentPosition((position) => {
                const { latitude, longitude } = position.coords;
                fetchWeatherDataByCoords(latitude, longitude);
            });
        };
        ```
        
2.  Fetch Weather Data by Coordinates
    *   Type:
        ```tsx
        // Function to fetch weather data using coordinates
        ```
    *   Start typing:
        ```tsx
        const fetchWeatherDataByCoords = async (lat: number, lon: number) => {
        ```
    *   Copilot Suggestion:
        ```tsx
            const response = await fetch(
                `https://api.openweathermap.org/data/2.5/weather?lat=${lat}&lon=${lon}&appid=${process.env.REACT_APP_WEATHER_API_KEY}&units=${units}`
            );
            const data = await response.json();
            setWeatherData(data);
        };
        ```

---------------
[Previous - Building the weather app core](./02-building-the-weather-app-core.md) |  [Next - State management with react hooks](./04-state-management-with-react-hooks.md)