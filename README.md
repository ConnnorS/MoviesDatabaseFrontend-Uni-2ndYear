# Movie Database React Client (Client-Side)

This project is a **React-based web application** that serves as the client for a movie database REST API, developed as part of my second-year CAB230 coursework. It allows users to search for movies, view detailed information, explore actor profiles, and access authenticated content via a secure login system.

The application communicates with the provided API entirely in the background, giving users a seamless browsing experience.

---

## Features Implemented

### Core Technologies
- **React.js** for UI and state management
- **Ag-Grid-React** for displaying and interacting with large movie datasets
- **React Router** for page navigation
- **React-ChartJS-2** for data visualisation
- **JSON Web Tokens (JWT)** for authentication

### API Endpoints Utilised
- `GET /movies/search` – Search for movies by title and/or year with pagination
- `GET /movies/data/{imdbID}` – View detailed movie information, including cast and ratings
- `GET /people/{id}` – View actor details and filmography (authentication required)
- `POST /user/register` – Create a new user account
- `POST /user/login` – Authenticate a user and retrieve tokens
- `POST /user/refresh` – Refresh authentication tokens automatically in the background
- `POST /user/logout` – Log out and clear tokens

### UI & Navigation
- Always-visible navigation bar with dynamic login/logout state
- Paginated and searchable movie table
- Clickable rows for quick navigation to movie or actor details
- Chart visualisation of actor IMDB rating distribution
- Minimalist layout for clarity and usability

---

## Skills Learned

By completing this project, I developed and strengthened skills in:

- **Frontend Development:** Building responsive and interactive UIs with React
- **API Integration:** Consuming REST endpoints and handling asynchronous requests
- **Authentication Handling:** Managing JWTs, token refresh, and protected routes
- **Component Libraries:** Implementing Ag-Grid for complex tabular data
- **Data Visualisation:** Creating charts with React-ChartJS-2
- **Routing:** Using React Router for multi-page SPA navigation
- **UI/UX Design:** Applying accessibility guidelines and dynamic UI states
- **Debugging & Testing:** Identifying, fixing, and documenting bugs and edge cases

---

## Limitations & Areas for Improvement
- **UI Responsiveness:** Some elements do not fully adapt to all screen sizes
- **Error Handling:** Certain input validation cases (e.g., invalid year search) need refinement
- **Navigation Flow:** Redirects for unauthenticated actor profile access could be improved to return users to their last viewed movie

---

## License
Data provided by OMDb, licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/).