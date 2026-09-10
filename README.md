# StudyMate AI

A complete, self-contained college-project demo web app.

## What is included

- Dashboard with connected study data
- Local AI Tutor with learning modes
- Subject/topic database
- Smart Notes
- AI-style flashcard generation
- Interactive quizzes with explanations
- Weak-topic detector
- Study Planner + calendar
- Exam Preparation + countdown
- Focus Timer
- Progress analytics + achievements
- Study History
- Global search
- Profile/settings
- Light/dark/system theme
- Guest/demo mode
- Responsive desktop/tablet/mobile UI
- PWA manifest + service worker

## Run on a laptop

### Easiest
1. Extract the ZIP.
2. Double-click `index.html`.
3. The app opens in your browser.

### Recommended for PWA/offline service-worker testing
If Python is installed:
1. Open Terminal/Command Prompt in this folder.
2. Run:
   `python -m http.server 8000`
3. Open:
   `http://localhost:8000`

Or with Node:
`npx serve .`

## Run on a phone

### Same Wi-Fi method
1. On the laptop, run `python -m http.server 8000 --bind 0.0.0.0`
2. Find the laptop's local IP address (for example `192.168.1.10`).
3. On the phone connected to the same Wi-Fi, open:
   `http://192.168.1.10:8000`
4. Use the browser's "Add to Home Screen" option.

For a public mobile install, deploy the folder to a static HTTPS host such as GitHub Pages, Netlify, Vercel, or Cloudflare Pages, then open it on the phone and use "Add to Home Screen".

## Important project note

This version intentionally uses a local, deterministic AI-style tutor/question engine so it runs without an API key or backend. User data is stored in the browser's `localStorage`.

For a production app with real AI, authentication, private cloud storage, PDF OCR, and secure multi-user accounts, add a backend and keep API keys on the server—not inside `index.html`.

## Demo flow

1. Sign in with the prefilled demo account.
2. Dashboard → see personalized recommendation.
3. AI Tutor → ask "Explain quadratic equations simply."
4. Quizzes → Practice Weak Topic.
5. Finish quiz → result and weak-topic analysis.
6. Planner → add revision task.
7. Focus Timer → start a 25-minute session.
8. Progress → see study time, mastery, and achievements.
