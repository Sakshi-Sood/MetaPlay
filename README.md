# MetaPlay

A modern movie streaming application built with React and Vite that provides seamless movie discovery with real-time search, trending movies tracking, and a beautiful user interface.

## Features

- **Real-time Movie Search**: Search through thousands of movies with debounced input for optimal performance
- **Trending Movies**: Track and display the most searched movies dynamically
- **Responsive Design**: Fully responsive interface that works on all devices
- **Modern UI**: Clean and intuitive design with smooth animations and loading states
- **Smart Search Tracking**: Automatically tracks search patterns and popular movies using Appwrite backend

## Tech Stack

- **Frontend Framework**: React 18
- **Build Tool**: Vite
- **Backend Services**: Appwrite (Database & Analytics)
- **Movie Data API**: The Movie Database (TMDB) API
- **Styling**: Tailwind CSS
- **State Management**: React Hooks (useState, useEffect)
- **Utilities**: react-use (for debouncing)

## Installation

### Prerequisites

- Node.js and npm installed on your machine.
- A TMDb API key. You can get one by creating an account on the TMDb website.

### Steps

1. Clone the repository:

```bash
git clone https://github.com/aditya-2k23/movie-app.git
```

2. Navigate to the project directory:

```bash
cd movie-app
```

3. Install the dependencies:

```bash
npm install
```

4. Create a `.env.local` file in the root of the project and add the following environment variables:

```env
VITE_TMDB_API_KEY=Your TMDb API key.
VITE_APPWRITE_PROJECT_ID=Your Appwrite project ID.
VITE_APPWRITE_DATABASE_ID=Your Appwrite database ID.
VITE_APPWRITE_COLLECTION_ID=Your Appwrite collection ID.
```

5. Start the development server:

```bash
npm run dev
```

6. Open the browser and go to `http://localhost:3000` to view the application.

#### Optional steps

7. To build the project for production, run:

```bash
npm run build
```

8. To preview the production build, run:

```bash
npm run serve
```

9. Lint the code:

```bash
npm run lint
```


## Configuration

### TMDB API Setup
1. Visit [TMDB website](https://www.themoviedb.org/)
2. Create an account and navigate to API settings
3. Generate an API Read Access Token
4. Add the token to your `.env` file

### Appwrite Setup
1. Create an account at [Appwrite Cloud](https://cloud.appwrite.io/)
2. Create a new project
3. Set up a database with a collection
4. Configure collection attributes as mentioned above
5. Add the IDs to your `.env` file

