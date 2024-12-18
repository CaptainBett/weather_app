# Captain's Weather App

🌤️ **Captain's Weather App** is a simple web application built using Flask that allows users to search for and view weather details for any city by providing its name and country code. The app fetches real-time weather data using the OpenWeatherMap API and displays it in an elegant, responsive interface.

## Features

- Fetch current weather details, including:
  - Temperature
  - Humidity
  - Wind speed
  - Sunrise and sunset times
  - General weather conditions (e.g., Rain, Clear, Clouds)
- Responsive and visually appealing UI using Bootstrap 5.
- Search weather by city name and country code.
- Displays formatted date and time information.

---

## Prerequisites

- Python 3.7+
- OpenWeatherMap API Key (Sign up at [OpenWeatherMap](https://openweathermap.org/) to get an API key.)

---

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/CaptainBett/weather_app.git
   cd weather_app
   ```

2. **Set up a Virtual Environment (Optional):**

   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. **Install Dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up Environment Variables:**

   - Create a `.env` file in the project directory.
   - Add the following line to the `.env` file:
     ```env
     API_KEY=your_openweathermap_api_key
     ```

5. **Run the Application:**
   ```bash
   python app.py
   ```
   The application will be available at `http://127.0.0.1:8000/`.

---

## Project Structure

```plaintext
├── app.py               # Flask application entry point
├── weather.py           # Helper functions for weather data fetching
├── templates
│   └── index.html       # Main HTML template
├── static               # Static assets (CSS, JS, images)
├── requirements.txt     # Python dependencies
└── .env                 # Environment variables (not included in repo)
```

---

## Usage

1. Open the application in your browser at `http://127.0.0.1:8000/`.
2. Enter the city name and its corresponding country code (e.g., `US` for the United States).
3. Click on the **Search** button.
4. View the weather details displayed on the page.

---

## Example

- **Input:**
  - City: `Nairobi`
  - Country Code: `KE`
- **Output:**
  - Weather: Clear skies
  - Temperature: 24°C
  - Humidity: 50%
  - Wind Speed: 5 m/s
  - Sunrise: 6:30 AM
  - Sunset: 6:45 PM

---

## Technologies Used

- **Backend:** Python, Flask
- **Frontend:** HTML, Bootstrap 5
- **API:** OpenWeatherMap

---

## Known Issues

- The application does not handle API rate limits gracefully.
- Error handling for invalid city names or country codes needs improvement.

---

## Future Enhancements

- Add support for additional weather data such as hourly forecasts.
- Improve error messages and handling for edge cases.
- Include historical weather data.

---

## License

This project is licensed under the MIT License.

---

## Acknowledgments

- [OpenWeatherMap](https://openweathermap.org/) for their fantastic API.
- [Bootstrap](https://getbootstrap.com/) for the responsive design framework.

---

## Screenshots

### Main Page

![Main Page](static/captain's%20weather.png.png)

---

Feel free to contribute, raise issues, or suggest enhancements for this project!
