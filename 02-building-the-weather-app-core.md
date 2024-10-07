# Section 2: Building the Weather App Core

**Time:** 25 minutes


## Objectives:

*   Set up the basic layout with CSS.
*   Integrate OpenWeatherMap API.
*   Utilize GitHub Copilot for API calls.


## Activities and GitHub Copilot Prompts:


### 2.1. Set Up Basic Layout

1.  Create a Basic Layout in `App.tsx`
    *   Type the following comment:
        ```tsx
        // Create a basic layout with a header and main section
        ```
    *   Start typing:
        ```tsx
        return (
        ```
    *   Copilot Suggestion:
        ```tsx
            <div className="App">
                <header className="App-header">
                    <h1>Weather App</h1>
                </header>
                <main>
                    {/* Main content will go here */}
                </main>
            </div>
        );
        ```
        
2.  Apply Basic Styles in `App.css`
    *   Type the following comment:
        ```css
        /* Style the App component */
        ```
    *   Start typing:
        ```css
        .App {
        ```
    *   Copilot Suggestion:
        ```css
            text-align: center;
        }
        ```


### 2.2. Integrate OpenWeatherMap API

1.  Obtain API Key
    *   Sign up at [OpenWeatherMap](https://openweathermap.org/) to get an API key.

2.  Store API Key in Environment Variable
    *   Create a `.env` file:
        ```bash
        touch .env
        ```
    *   Add the API key:
        ```env
        REACT_APP_WEATHER_API_KEY=your_api_key_here
        ```
        
3.  Fetch Weather Data
    *   In `App.tsx`, type:
        ```tsx
        // Function to fetch weather data for a city
        ```
    *   Start typing:
        ```tsx
        const fetchWeatherData = async (city: string) => {
        ```
    *   Copilot Suggestion:
        ```tsx
            const response = await fetch(
                `https://api.openweathermap.org/data/2.5/weather?q=${city}&appid=${process.env.REACT_APP_WEATHER_API_KEY}&units=metric`
            );
            const data = await response.json();
            setWeatherData(data);
        };
        ```
        
4.  Handle User Input
    *   Add a state variable for the city:
        ```tsx
        const [city, setCity] = useState<string>("");
        ```
    *   Create an input field:
        ```tsx
        // Input field for the city
        ```
    *   Copilot Suggestion:
        ```tsx
        <input
            type="text"
            value={city}
            onChange={(e) => setCity(e.target.value)}
            placeholder="Enter city"
        />
        <button onClick={() => fetchWeatherData(city)}>Get Weather</button>
        ```
