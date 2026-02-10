# Film Discovery Platform

A full-stack web application for discovering and tracking movies, TV shows, and actors. Built with React, TypeScript, and Firebase, integrating The Movie Database (TMDB) API for comprehensive entertainment content.
![Home Page](src/images/homePage.png)
![Movies Page](src/images/moviesPage.png)
![Movie Details Page](src/images/movieDetailsPage.png)

## Features

### Content Discovery
- **Universal Search** - Search across movies, TV shows, and actors from a centralized search bar
- **Trending Content** - Toggle between daily and weekly trending entertainment
- **Categorized Browsing** - Filter content by top rated, newest releases, and other categories
- **Full Pagination** - Navigate large datasets efficiently

### Content Details
- **Rich Media Pages** - Detailed information for movies, TV shows, and actors
- **Cast Information** - View top cast members and their filmographies
- **User Reviews** - Read community reviews in an integrated modal interface
- **Similar Content** - Discover related movies and shows

### User Features
- **Firebase Authentication** - Secure user registration and login
- **Favorites Management** - Save and organize favorite content with persistent storage
- **User Profiles** - Track favorites, registration date, and activity
- **Dream Movie Creator** - Build custom movie concepts with cast selection
- **Dark Mode** - Toggle between light and dark themes

## Tech Stack

**Frontend:**
- React with TypeScript
- Material-UI (MUI) component library
- React Router for navigation

**Backend & Data:**
- Firebase Authentication
- Cloud Firestore for data persistence
- TMDB API for entertainment data

## Setup

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Firebase project with Firestore enabled
- TMDB API key

### Installation

1. Clone the repository
```bash
git clone https://github.com/D-Sills/film-discovery-app.git
cd film-discovery-app
```

2. Install dependencies
```bash
npm install
```

3. Create a `.env` file in the root directory with your API keys:
```
REACT_APP_TMDB_KEY=your_tmdb_api_key
REACT_APP_FIREBASE_API_KEY=your_firebase_api_key
REACT_APP_FIREBASE_AUTH_DOMAIN=your_firebase_auth_domain
REACT_APP_FIREBASE_PROJECT_ID=your_firebase_project_id
REACT_APP_FIREBASE_STORAGE_BUCKET=your_firebase_storage_bucket
REACT_APP_FIREBASE_MESSAGING_SENDER_ID=your_firebase_messaging_sender_id
REACT_APP_FIREBASE_APP_ID=your_firebase_app_id
```

4. Start the development server
```bash
npm start
```

The application will open at `http://localhost:3000`

## TMDB API Endpoints Used

- `/movie/{movie_id}` - Movie details
- `/movie/{movie_id}/reviews` - Movie reviews
- `/movie/{movie_id}/similar` - Similar movies
- `/movie/{movie_id}/credits` - Movie cast
- `/tv/{category}` - TV show categories
- `/tv/{tv_id}` - TV show details
- `/tv/{tv_id}/credits` - TV show cast
- `/tv/{tv_id}/reviews` - TV show reviews
- `/person/popular` - Popular actors
- `/person/{person_id}` - Actor details
- `/person/{person_id}/combined_credits` - Actor filmography
- `/trending/all/{time_window}` - Trending content
- `/search/multi` - Universal search