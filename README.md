# Vocham

Vocham is a student blogging platform originally built for high school students to publish news, articles, interviews, and opinion pieces. It was actively used by the school as its student-run publication.

The project is no longer in active use by the school, but it remains live as part of my personal portfolio, showcasing a full-featured content platform built with React and Firebase.

🔗 [vocham.com](https://vocham.com/)

## Features

- **Blog posts** — create, edit, and read articles with a rich text editor (Draft.js)
- **Categories & tags** — browse content by topic
- **Author profiles** — dedicated pages for each contributing student writer
- **Comments** — reader discussion on posts
- **Bookmarks** — save posts to read later
- **User accounts** — sign up, log in, and password recovery
- **Popular posts widget** — highlights trending articles
- **Contact form** — powered by EmailJS
- **SEO & social meta tags** — per-page metadata for better sharing/discoverability
- **Dark mode** toggle

## Tech Stack

- **React 18** (bootstrapped with Create React App / `react-scripts`)
- **Firebase** (Firestore) as the backend
- **Redux** + Redux Thunk for state management
- **React Router v5** for routing
- **Ant Design**, **Material UI**, **React Bootstrap**, **Semantic UI React** for UI components
- **Draft.js** for the post editor
- **EmailJS** for the contact form
- **react-snapshot** for pre-rendering static pages at build time

## Getting Started

### Prerequisites

- Node.js and npm

### Installation

```bash
npm install
```

### Development

```bash
npm start
```

Runs the app in development mode on [http://localhost:3006](http://localhost:3006).

### Build

```bash
npm run build
```

Builds the app for production to the `build` folder and pre-renders pages with `react-snapshot`.

### Tests

```bash
npm test
```

## Configuration

The app connects to a Firebase project for data storage. Firebase credentials are configured in `src/firebase-config.js`.

## Project Structure

```
src/
├── Api/            # Firestore/API controllers (posts, bookmarks)
├── actions/         # Redux actions
├── reducers/        # Redux reducers
├── services/        # Auth service
├── helpers/         # Utility helpers
├── components/      # Reusable UI components (blog, comments, header, footer, etc.)
├── pages/            # Route-level pages (home, login, sign up, author, account, etc.)
└── firebase-config.js
```

## About the Project

Vocham started as a way for students to get real-world experience writing and publishing online, giving them a shared voice to write about the things they cared about. Today it lives on as a demonstration of a complete blog platform — authentication, content management, and reader engagement features — built end-to-end in React.
