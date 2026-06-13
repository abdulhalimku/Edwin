# Edwin 🌤️

**Programer Front-End Developer** | Indonesia

A collection of web development projects showcasing modern frontend skills with vanilla JavaScript, React, and responsive design.

---

## 📂 Featured Projects

### 🌤️ Weather App

A simple and responsive weather application built with vanilla JavaScript using the Fetch API and async/await. Search for real-time weather data for any city in the world.

![Weather App Preview](https://via.placeholder.com/800x400?text=Weather+App+Preview)

#### ✨ Features

- 🔍 Search weather by city name
- 🌡️ Displays temperature in Celsius
- 💧 Shows humidity percentage
- 💨 Shows wind speed
- ⚠️ Error handling for invalid city names
- ⌨️ Press Enter to search (keyboard friendly)
- 📱 Responsive design for mobile and desktop

#### 🛠️ Built With

| Technology | Purpose |
|---|---|
| HTML5 | Page structure |
| CSS3 | Styling & responsive layout |
| JavaScript (ES6+) | Logic & DOM manipulation |
| Fetch API | HTTP requests |
| async/await | Asynchronous handling |
| OpenWeatherMap API | Weather data source |

#### 📁 Project Structure

```
weather-app/
├── index.html      # Main HTML structure
├── style.css       # Styling and responsive layout
├── script.js       # Fetch logic and DOM rendering
└── README.md       # Project documentation
```

#### 📸 Screenshots

| Desktop | Mobile |
|---|---|
| ![Desktop](https://via.placeholder.com/380x220?text=Desktop+View) | ![Mobile](https://via.placeholder.com/180x320?text=Mobile+View) |

---

### 👨‍💻 Portfolio Website

A modern, minimal portfolio showcasing projects, skills, and contact information with a terminal-inspired design.

#### 🎨 Design Features

- Cyberpunk-inspired dark theme with cyan accents
- Sticky navigation bar
- Animated terminal window
- Responsive grid layouts
- Smooth hover interactions
- Mobile-optimized design

#### 📂 Includes Sections

- **Hero Section** - Introduction with CTA buttons
- **Statistics** - Experience, projects completed, remote readiness
- **Technical Skills** - Organized skill cards with proficiency levels
- **Featured Projects** - Portfolio grid with project descriptions
- **Contact Section** - Call-to-action with social links
- **Footer** - Copyright and branding

---

## ⚙️ Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge)
- A free API key from [OpenWeatherMap](https://openweathermap.org/api)
- A code editor (VS Code, Sublime, etc.)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/abdulhalimku/Edwin.git
   cd Edwin
   ```

2. **For Weather App**
   - Get your API key from [openweathermap.org](https://openweathermap.org/api)
   - Open `script.js` and replace the placeholder:
     ```js
     const API_KEY = "YOUR_API_KEY_HERE"; // ← paste your key here
     ```

3. **Run the project**
   - Open `index.html` with [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in VS Code
   - Or simply open in your browser

---

## 📖 How It Works

### Weather App Flow

```
User types city name
        ↓
getCuaca() is called
        ↓
fetch() sends request to OpenWeatherMap API
        ↓
await response.json() parses the data
        ↓
DOM is updated with weather info
        ↓
try/catch handles any network or API errors
```

### Core async/await logic

```js
async function getCuaca() {
  try {
    const res = await fetch(`${BASE_URL}?q=${kota}&appid=${API_KEY}&units=metric`);
    if (!res.ok) throw new Error("City not found");
    const data = await res.json();
    // render data to DOM
  } catch (error) {
    // display error message
  }
}
```

---

## 🌐 API Reference

This project uses the [OpenWeatherMap Current Weather API](https://openweathermap.org/current).

| Parameter | Value |
|---|---|
| Endpoint | `https://api.openweathermap.org/data/2.5/weather` |
| Method | `GET` |
| Auth | `appid` query parameter |
| Units | `metric` (Celsius) |

---

## 🔮 Future Improvements

- [ ] 5-day weather forecast
- [ ] Weather icons from API
- [ ] Save recent searches to localStorage
- [ ] Toggle between Celsius and Fahrenheit
- [ ] Detect user location automatically (Geolocation API)
- [ ] Add more projects to portfolio
- [ ] Integrate blog section
- [ ] Add dark/light theme toggle

---

## 👤 About Me

**Abdul Halim** | Web Developer based in Indonesia

### 🎯 Skills

- **Frontend**: React.js, HTML5, CSS3, JavaScript (ES6+), Tailwind CSS
- **Backend**: Node.js, PHP, Laravel
- **Database**: MySQL
- **Tools**: Git, GitHub, VS Code

### 📊 Stats

- 3+ Years Experience
- 20+ Projects Completed
- 100% Remote Ready

---

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

---

## 📧 Contact & Links

- **Email**: [abdulkhalimku@gmail.com](mailto:abdulkhalimku@gmail.com)
- **GitHub**: [@abdulhalimku](https://github.com/abdulhalimku)
- **LinkedIn**: [Your LinkedIn Profile](https://linkedin.com/in/yourprofile)

---

> Built as part of my frontend web development learning journey — practicing Fetch API, async/await, DOM manipulation, and responsive design.
