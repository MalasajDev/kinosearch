# 🌐 Website Link

https://kinosearch-alpha.vercel.app/

# 🎬 KinoSearch

**KinoSearch** — a modern web application for searching movies and TV series, viewing detailed information, saving favorites, and working with reviews. The project is built as a complete SPA showcase: with a clean architecture, responsive interface, animations, and integration with an external API.

---

## ✨ What the application can do

- 🔎 Search for movies and TV series through **Open Movie Database (OMDb) API**
- 🎞️ Open a detailed movie card: poster, rating, genres, description, actors, director, awards, and other data
- ❤️ Add movies to favorites and keep them between sessions
- 🕘 Save search query history
- 📝 Read and add user reviews for movies
- 🌌 Display a cinematic dark interface with an animated background
- 📱 Work correctly on mobile devices, tablets, and desktops
- ⚠️ Handle loading states, errors, empty results, and missing posters

---

## 🚀 Demo scenario

The user opens the home page, sees collections and a visual hero section, searches for a movie or TV series, opens its card, explores the details, adds the movie to favorites, and leaves a review. All key actions are saved locally, so the application feels like a finished product rather than just a test page with an API request.

---

## 🛠️ Technology stack

| Technology       | Purpose                                      |
| ---------------- | -------------------------------------------- |
| **React 18**     | Component-based UI                           |
| **TypeScript**   | Typing for data, API, and state              |
| **Vite**         | Fast build and dev server                    |
| **React Router** | Client-side routing                          |
| **Zustand**      | Global state and persistence in localStorage |
| **Axios**        | Requests to the OMDb API                     |
| **Tailwind CSS** | Responsive styling                           |
| **GSAP**         | Smooth UI animations                         |
| **Three.js**     | Visual animated background                   |
| **OMDb API**     | Data about movies and TV series              |

---

## 🧩 Main pages

| Page         | Route           | Description                                                  |
| ------------ | --------------- | ------------------------------------------------------------ |
| 🏠 Home      | `/`             | Hero section, collections, genres, and popular content       |
| 🔎 Search    | `/search?q=...` | Movie and TV series search with results in a responsive grid |
| 🎬 Details   | `/movie/:id`    | Full information about the selected movie or TV series       |
| ❤️ Favorites | `/favorites`    | Movies saved by the user                                     |
| 🚧 404       | `*`             | Page for nonexistent routes                                  |

---

## 📁 Project structure

```text
src/
├── api/                 # OMDb API, types, and data normalization
├── components/
│   ├── layout/          # Header, Footer
│   ├── sections/        # Main page sections
│   └── ui/              # Reusable UI components
├── data/                # Initial data for reviews
├── hooks/               # Hooks for search, loading, and infinite scroll
├── pages/               # Application pages
├── store/               # Zustand store
├── utils/               # Constants, formatters, fallback logic
├── App.tsx              # Application routing
└── main.tsx             # Entry point
```

---

## ⚙️ Quick local start

### 1. Install dependencies

```bash
npm install
```

### 2. Create `.env`

You can use `.env.example` as a template:

```env
VITE_OMDB_API_KEY=your_api_key_here
VITE_OMDB_BASE_URL=https://www.omdbapi.com/
```

You can get an API key on the [OMDb API](https://www.omdbapi.com/apikey.aspx) website.

### 3. Run the project

```bash
npm run dev
```

The application will be available at:

```text
http://localhost:5173
```

---

## 📦 Available commands

| Command           | Description                           |
| ----------------- | ------------------------------------- |
| `npm run dev`     | Start the dev server                  |
| `npm run build`   | TypeScript check and production build |
| `npm run preview` | Preview the production build          |
| `npm run lint`    | Check the code with the linter        |

---

## 🔐 Environment variables

```env
VITE_OMDB_API_KEY=your_api_key_here
VITE_OMDB_BASE_URL=https://www.omdbapi.com/
```

⚠️ A real API key should not be committed to the repository. Use `.env.example` as a configuration example.

---

## 🧪 Build

```bash
npm run build
```

After a successful build, the production files will be located in the `dist/` folder. The project can be deployed to Vercel, Netlify, GitHub Pages, or any other static hosting.

---

## 👨‍💻 Author's note

KinoSearch was created as a demo frontend project with a focus on clean structure, pleasant user experience, and working with real data. This application can be developed further: add authentication, personal collections, recommendations, trailers, server-side review storage, and a full backend.

**KinoSearch — a small but complete movie product that shows not only command of the stack, but also attention to detail.** 🍿
