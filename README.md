# My Website

# Folder Structure
portfolio-site/
├── my-app/                          # React frontend (CRA + TypeScript)
│   ├── public/
│   │   ├── images/
│   │   │   ├── smiskis/             # SVG/PNG Smiski variants
│   │   │   └── albums/              # Album art
│   │   └── index.html
│   ├── src/
│   │   ├── components/
│   │   │   ├── smiskis/             # 🟢 Modular Smiski system
│   │   │   │   ├── SmiskiBase.tsx
│   │   │   │   ├── SmiskiThinker.tsx
│   │   │   │   ├── SmiskiLifter.tsx
│   │   │   │   ├── SmiskiSleeper.tsx
│   │   │   │   └── index.ts
│   │   │   ├── NowPlaying.tsx       # 🎵 Now Playing widget
│   │   │   ├── PRBoard.tsx          # 💪 Gym PR noticeboard
│   │   │   ├── ProjectGallery.tsx   # 📁 Gallery component
│   │   │   ├── ProjectCard.tsx      # 📦 Individual project card
│   │   │   ├── ThemeProvider.tsx    # 🌙 Theme + dark mode context
│   │   │   └── Navbar.tsx
│   │   ├── data/
│   │   │   ├── projects.ts          # List of projects (manual or fetched)
│   │   │   └── pr_data.ts           # Gym PRs
│   │   ├── hooks/
│   │   │   ├── useDarkMode.ts       # Dark mode context or media query hook
│   │   │   └── useNowPlaying.ts     # Fetch Spotify/JSON Now Playing
│   │   ├── App.tsx                  # 🔁 Central layout
│   │   ├── index.tsx
│   │   ├── react-app-env.d.ts
│   │   └── styles/
│   │       └── globals.css          # Tailwind base + glow styles
│   ├── tailwind.config.js
│   ├── tsconfig.json
│   └── package.json
│
├── backend/                         # FastAPI backend
│   ├── app/
│   │   ├── main.py
│   │   ├── routers/
│   │   │   ├── now_playing.py
│   │   │   └── pr_board.py
│   │   └── utils/
│   │       └── spotify.py
│   └── requirements.txt
│
├── shared/
│   ├── projects.json                # Shared data for backend/frontend
│   ├── pr_data.json
│   └── now_playing_fallback.json
│
├── .gitignore
├── README.md
└── LICENSE