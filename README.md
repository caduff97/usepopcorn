# 🎬 usePopcorn: Movie Ratings App

This project is a **React application** for searching movies, tracking what you've watched, and rating them. It utilizes the [OMDb API](https://www.omdbapi.com/) to fetch movie details. This app allows users to search for movies, view movie details, and maintain a list of watched movies with custom ratings.

## Features

- **Movie Search**: Search for movies using the OMDb API.
- **Watched List**: Add movies to a watched list with custom user ratings.
- **Movie Details**: View detailed information about each movie, including IMDb ratings, plot, actors, and more.
- **Persistent State**: Watched movies and ratings are saved in local storage, ensuring data is kept across sessions.
- **Responsive Design**: The UI adapts for various screen sizes.

## Tech Stack

- **React**: Main framework for the UI.
- **Hooks**: Custom hooks (`useMovies`, `useLocalStorageState`, `useKey`) to manage movie fetching, local storage, and keyboard event handling.
- **OMDb API**: Fetches movie data and details.
- **LocalStorage**: Persists the watched list and user ratings.
- **CSS**: Basic styling for the UI components.

## Installation

To run the app locally:

1.  Clone the repository:
    `git clone https://github.com/your-username/usepopcorn.git`

2.  Navigate to the project directory:
    `cd usepopcorn`
3.  Install dependencies:
    `npm install`
4.  Start the app:
    `npm start`
5.  Open your browser and go to http://localhost:3000.

## Project Structure

- **`/src`**: The main source folder with components and custom hooks.
  - **`App.js`**: The main component where all other components come together.
  - **`useMovies.js`**: A custom hook for fetching movies from the OMDb API.
  - **`useLocalStorageState.js`**: A custom hook for persisting state in localStorage.
  - **`useKey.js`**: A custom hook for handling key presses (e.g., "Enter" to clear search).
  - **`StarRating.js`**: A component for user ratings with stars.
  - **`MovieList.js`**: Component to list the movies from the search results.
  - **`MovieDetails.js`**: Component to display detailed information about a selected movie.
  - **`WatchedMoviesList.js`**: A component to show the user's watched movies with ratings.

## API

The app fetches movie data from the [OMDb API](http://www.omdbapi.com/). You need to sign up for an API key to get started.

Replace the placeholder API key in `App.js` with your own:
`const KEY = "your_omdb_api_key";`

## Future Improvements

- **Responsive Enhancements**: Further improvements to the layout for better user experience on smaller devices.
- **Pagination**: Add pagination for the search results to handle large datasets.
- **Improved State Management**: Integrate a more robust state management solution like Redux for better scalability.
- **Authentication**: Add user accounts to save watched movies across different devices.
- **Backend Integration**: Connect to a backend service for storing movie data and user preferences.
