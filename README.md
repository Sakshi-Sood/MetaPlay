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

## Prerequisites

Before you begin, ensure you have the following installed:
- Node.js (v14.0.0 or higher)
- npm or yarn package manager
- An Appwrite account and project setup
- TMDB API key

## 🛠️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/metaplay.git
   cd metaplay
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```
   or
   ```bash
   yarn install
   ```

3. **Set up environment variables**
   
   Create a `.env` file in the root directory and add the following:
   ```env
   VITE_TMDB_API_KEY=your_tmdb_api_key_here
   VITE_APPWRITE_PROJECT_ID=your_appwrite_project_id
   VITE_APPWRITE_DATABASE_ID=your_database_id
   VITE_APPWRITE_COLLECTION_ID=your_collection_id
   ```

4. **Configure Appwrite Database**
   
   Create a collection in your Appwrite database with the following attributes:
   - `searchTerm` (string, required)
   - `count` (integer, required, default: 1)
   - `movie_id` (integer, required)
   - `poster_url` (string, required)

## 🏃‍♂️ Running the Application

### Development Mode
```bash
npm run dev
```
or
```bash
yarn dev
```
The application will start on `http://localhost:5173`

### Production Build
```bash
npm run build
```
or
```bash
yarn build
```

### Preview Production Build
```bash
npm run preview
```
or
```bash
yarn preview
```

## 📁 Project Structure

```
metaplay/
├── public/
│   ├── hero-img.png
│   ├── metaplay.png
│   ├── no-movie.png
│   ├── search.svg
│   └── star.svg
├── src/
│   ├── components/
│   │   ├── MovieCard.jsx    # Individual movie card component
│   │   ├── Navbar.jsx        # Navigation header
│   │   ├── Search.jsx        # Search input component
│   │   └── Spinner.jsx       # Loading spinner
│   ├── App.jsx               # Main application component
│   ├── appwrite.js           # Appwrite configuration and functions
│   ├── main.jsx              # Application entry point
│   └── index.css             # Global styles
├── .env                      # Environment variables (create this)
├── .gitignore
├── index.html
├── package.json
├── README.md
└── vite.config.js
```

## 🔧 Configuration

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

## 🙏 Acknowledgments

- [TMDB](https://www.themoviedb.org/) for providing the movie database API
- [Appwrite](https://appwrite.io/) for backend services
- [Vite](https://vitejs.dev/) for the blazing fast build tool
- [React](https://reactjs.org/) for the UI library


**Happy Streaming! 🍿**