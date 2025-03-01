Here's a README template for your project:

---

# usePopcorn

`usePopcorn` is a simple React application that allows users to search for movies, view their details, rate them, and add them to a watched list. The app also provides an average rating and runtime for the movies the user has watched

## Features

- **Search Movies**: Search for movies by title using the OMDB API
- **Movie Details**: View details of a selected movie, including its runtime, director, actors, and plot.
- **Rating**: Rate movies from 1 to 10 stars.
- **Watched List**: Add movies to the watched list and see your average ratings and runtime for watched movies.
- **Interactive UI**: Clean user interface with a flexible layout and animated transitions

## Setup

### Prerequisites

Before getting started, make sure you have the following installed on your machine:

- **Node.js** (Download it from [here](https://nodejs.org/)).
- **npm** (Node Package Manager) (It comes with Node.js).

### Installing

1. Clone the repository:
   ```bash
   git clone https://github.com/suryanag9099/use-popcorn.git
   ```

2. Navigate into the project directory:
   ```bash
   cd use-popcorn
   ```

3. Install the dependencies:
   ```bash
   npm install
   ```

4. To run the app in development mode:
   ```bash
   npm start
   ```

   The app will be available in your browser at `http://localhost:3000`.

## Usage

1. **Search**: Type the name of a movie in the search bar, and it will fetch movie data from the OMDB API.
2. **Movie Details**: Click on a movie from the search results to view its details, including runtime, genre, and plot.
3. **Rating**: Rate a movie from 1 to 10 stars. Once rated, you can add it to your "Watched" list.
4. **Watched Movies**: After adding movies to your watched list, you can see the average IMDb rating, user rating, and runtime for all the movies you've watched.

## Components

### `App`
- This is the main component that handles state, effects, and displays the `NavBar`, `Main`, and `MovieDetails` components.

### `NavBar`
- A component that contains the `Logo` and the `Search` bar, and displays the number of search results.

### `MovieList`
- Displays the list of movies fetched based on the search query.

### `MovieDetails`
- Displays detailed information about a selected movie and provides the option to rate and add it to the watched list.

### `WatchedSummary`
- Shows a summary of the watched movies, including the number of movies, average IMDb rating, average user rating, and average runtime.

### `WatchedMoviesList`
- Displays the list of movies in the watched list with an option to delete them.

### `StarRating`
- A component that lets users rate movies with a star rating system. It includes hover effects and shows the current rating.

### `Loader` and `ErrorMessage`
- Components to show loading status and error messages, respectively, when fetching data from the OMDB API.

## API

This app uses the [OMDB API](https://www.omdbapi.com/) to fetch movie data. You'll need to sign up for an API key and replace the value of `KEY` in the `App` component with your own API key. Currently, a sample key `c2e9b79e` is used, but it may not work if you exceed the request limits.

## Future Enhancements

- Improve the UI with animations and transitions.
- Add a user authentication system to save watched movies and ratings across sessions.
- Implement a movie recommendation feature based on the user's watched list.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to customize and add more details as needed. Let me know if you'd like any modifications!
