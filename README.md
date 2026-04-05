# 🎬 CineTrack — Advanced Movie Search & Watchlist App

CineTrack is a React-based movie application that enables users to search, explore, rate, and manage movies using real-time data from the OMDb API.

This project focuses on implementing **real-world frontend patterns**, including API optimization, side-effect management, and dynamic UI state handling.

---

## 🚀 Overview

CineTrack is designed to simulate a real production-like frontend application by handling:

- Asynchronous API communication
- Dynamic UI updates
- User interaction and state persistence (in-memory)
- Performance optimizations for better user experience

---

## Preview

<video controls src="cinetrack.mp4" title="CineTrack"></video>

https://github.com/user-attachments/assets/115eefe3-90c2-48e4-9dcc-02785aa81906



## ✨ Key Features

### 🔍 Smart Movie Search

- Triggers API calls only when input length ≥ 3
- Prevents unnecessary requests and improves performance
- Clears results when input is empty

---

### ⚡ Optimized API Handling

- Implements **request cancellation** to avoid race conditions
- Ensures only the latest search result is displayed
- Handles rapid user input efficiently

---

### 📄 Dynamic Movie Details Panel

- Fetches detailed movie data using `imdbID`

- Displays rich metadata:
  - Title, release date, runtime
  - Genre, plot, actors, director
  - IMDb rating

- Seamless toggle between list view and details view

---

### ⭐ Interactive Rating System

- Users can rate movies using a custom star rating component
- Enforces rating before adding to watchlist
- Enhances user engagement

---

### 📌 Watchlist Management

- Add movies to a watched list
- Remove movies dynamically
- Prevent duplicate entries

---

### 📊 Computed Watchlist Analytics

- Calculates:
  - Average IMDb rating
  - Average user rating
  - Average runtime

- Demonstrates data transformation and aggregation

---

### ⏳ Loading & Error Handling

- Displays loading indicator during API calls
- Handles:
  - API errors
  - Network failures
  - No results scenarios

---

### 🧠 Side Effect Management

Implements multiple real-world side effects:

- API calls based on state changes
- Cleanup of pending requests
- Keyboard event handling (Escape to close details)
- Dynamic document title updates

---

### 🎯 UI Behavior & UX Enhancements

- Conditional rendering based on application state
- Collapsible UI sections
- Smooth interaction flow
- Improved accessibility with keyboard support

---

## 🛠️ Tech Stack

- ⚛️ React (Functional Components)
- 🧩 Hooks (`useState`, `useEffect`)
- 🌐 Fetch API
- 🧠 AbortController (request cancellation)
- 🎨 CSS (layout and responsiveness)
- 🔐 Environment Variables

---

## ⚙️ Setup & Installation

```bash id="1p6b6s"
git clone https://github.com/SuryaTejaTangella/CineTrack.git
cd CineTrack
npm install
npm start
```

Create a `.env` file:

```env id="5c0qz8"
REACT_APP_OMDB_API_KEY=your_api_key_here
```

---

## 🧪 Edge Cases Considered

- Rapid typing (prevents stale API responses)
- Empty or short queries
- Missing or inconsistent API data
- Duplicate watchlist entries
- Network/API failures

---

## 🎯 What This Project Demonstrates

- Strong understanding of React hooks and lifecycle
- Handling asynchronous operations effectively
- Managing complex UI states (loading, error, success)
- Implementing performance optimizations
- Writing modular and maintainable components

---

## 🚧 Future Enhancements

- Persistent watchlist using localStorage
- Debounced search for further optimization
- Improved mobile responsiveness
- Dark mode support
- Backend proxy for secure API handling

---

## 👨‍💻 Author

**Surya Teja Tangella**

---

## ⭐ If you found this useful

Give this project a ⭐ and feel free to explore the code!
