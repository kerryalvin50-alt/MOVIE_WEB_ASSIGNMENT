# MOVIE_WEB_ASSIGNMENT
a  movie website created with javascript
# 🎬 CinePulse - Movie & TV Show Discovery Web Application

[![React](https://img.shields.io/badge/React-18.x-blue?style=for-the-badge&logo=react)](https://reactjs.org/)
[![Material UI](https://img.shields.io/badge/Material_UI-v5-007FFF?style=for-the-badge&logo=mui)](https://mui.com/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.x-38B2AC?style=for-the-badge&logo=tailwind-css)](https://tailwindcss.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**CinePulse** is a lightning-fast, modern movie and TV show discovery web application built using **React**, **Material UI (MUI v5)**, and **Tailwind CSS**. It connects to the **TMDB (The Movie Database) API** while providing a robust offline fallback mode with curated mock data so users can explore cinematic masterpieces instantly without requiring an API key on first launch.

---

## ✨ Key Features

- **🎥 Dual Data Engine (Live API + Smart Fallback):** Automatically queries the live TMDB API if a user provides an API key, or seamlessly falls back to a built-in mock dataset so the app works out-of-the-box.
- **🔍 Real-Time Search & Multi-Filtering:** Instantly filter movies and series by title, genre, release year, or rating with debounced live search queries.
- **⭐ Interactive Watchlist:** Save favorite movies and TV shows directly to local storage for quick access later.
- **🍿 Cinematic Details & Trailer Previews:** Click any movie card to open a rich detail modal featuring overviews, runtimes, vote averages, and embedded trailers.
- **🎨 Modern Dark-Themed UI/UX:** Styled with Tailwind CSS and Material UI components, complete with custom scrollbars, glassmorphism panels, card glow animations, and responsive layouts.

---

## 🛠️ How I Built It (Development Process)

CinePulse was engineered with a focus on **component modularity**, **zero-config initial user experience**, and **sleek modern design**.

### 1. Architecture & Tech Stack Selection
- **Frontend Framework:** React 18 (loaded via CDN using Babel Standalone for quick browser-based execution and easy sharing).
- **UI Component Libraries:** 
  - **Material UI (MUI v5)** for complex interactive components (Dialogs, Snackbars, Select dropdowns, Badges).
  - **Tailwind CSS** for fast layout scaffolding, spacing utilities, and flexbox/grid alignments.
- **Icons:** **Lucide Icons** for clean, modern iconography.
- **Fonts:** Google Fonts (`Inter` for clean body typography and `Montserrat` for bold, impactful titles).

### 2. State Management & Persistence
- Built a centralized React Context (`AppContext`) to manage application-wide states:
  - Active navigation tabs (`home`, `movies`, `tv`, `watchlist`).
  - Search queries and live filtering.
  - User watchlist sync with browser `localStorage`.
  - API key configuration and toast notification states.

### 3. Graceful Degradation & Offline Support
- To prevent blank screens or broken experiences for first-time visitors who haven't generated a TMDB API key yet, I implemented a **Fallback Mock Data Engine**. 
- The app intelligently checks if an API key is stored; if absent or if an API request fails, it switches to a curated dataset of top-rated modern films and series (e.g., *Dune: Part Two*, *Oppenheimer*, *Interstellar*, *Spider-Man: Across the Spider-Verse*).

### 4. Styling & Animations
- Custom CSS written in `style.css` provides:
  - Custom dark-themed scrollbars styled with slate and rose accents (`#e11d48`).
  - Smooth card translation and box-shadow glow effects (`.movie-card:hover`).
  - Backdrop blur gradients for the hero banner and fixed navigation header.

---

## 🚀 Getting Started Locally

Because this project utilizes Babel Standalone and script tags for rapid deployment, you can run it instantly without running complex node build steps:


STEPS ON HOW THE SITE IS OPERATED

---

### Step 1: Open the Application

1. Double-click your local `index.html` file or open the deployed link in any modern web browser (Chrome, Firefox, Edge, Safari).
2. The site will load instantly with a dark, cinematic theme featuring a navigation bar, a search bar, and a curated list of top movies.

### Step 2: Browse Movies and TV Shows

Use the left-hand sidebar or top menu to switch between different discovery sections:

* **🏠 Home:** Explore featured hero banners, trending lists, and top picks right on the main dashboard.
* **🎬 Movies:** Filter specifically through popular, action, sci-fi, and drama films.
* **📺 TV Shows:** Discover popular television series and serial dramas.

### Step 3: Search for Specific Titles

1. Click on the **Search bar** located at the top of the header.
2. Type the name of any movie, TV show, or keyword (e.g., *"Dune"*, *"Interstellar"*, or *"Sci-Fi"*).
3. Results will filter dynamically in real-time as you type.

### Step 4: View Detailed Information & Trailers

1. Click on any movie or TV show card to open the **Details Modal**.
2. Read the full synopsis, check the release date, runtime, genres, and overall vote average.
3. Click the **Watch Trailer** button to preview the official video trailer inside an interactive player popup.

### Step 5: Build Your Personal Watchlist

1. Found something you want to watch later? Click the **Bookmark / Add to Watchlist** icon on any movie card or inside the detail view.
2. Navigate to the **Watchlist** tab in the sidebar at any time to see all your saved titles stored securely in your browser.

### Step 6: Unlock Live Data with a TMDB API Key (Optional)

CinePulse comes with built-in mock data so it works instantly without setup. However, if you want access to thousands of live, up-to-date movies and shows:

1. Get a free API key from [The Movie Database (TMDB)](https://www.google.com/search?q=https://www.themoviedb.org/settings/api).
2. Click the **API Key / Settings** button in the app interface.
3. Paste your API key and save it to instantly switch from offline mode to live global database searching!
