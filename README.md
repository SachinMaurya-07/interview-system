# Intervue.ai — Mock Interview Practice

A browser-based mock interview practice app with role-specific question sets, voice input, speaking feedback, filler-word tracking, pacing indicators, and breathing exercises.

## Features

- Choose an interview role, seniority level, and session length
- Practice technical and behavioral interview questions
- Use browser speech recognition where supported
- Review answer feedback based on built-in question guidance and keywords
- Track session preferences/history stored in the browser
- Responsive interface with animated styling

## Tech stack

- HTML
- CSS
- Vanilla JavaScript
- Browser Web Speech API (where supported)
- Lucide icons and Google Fonts loaded from CDNs

## Run locally

No build step or package installation is required.

### Option 1: Open directly

Open `index.html` in a modern browser. Some browser speech features may be unavailable when opened from a local file.

### Option 2: Run a local web server (recommended)

With Python installed, run this from the project directory:

```bash
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

You can also use VS Code's Live Server extension.

## Browser compatibility and privacy

Speech recognition support varies by browser and operating system. Use a current browser that supports the Web Speech API, and grant microphone/speech permissions if prompted. HTTPS or localhost may be required for browser capabilities.

The app's question bank and answer evaluation logic are bundled in `interview.js`; this repository does not include a connection to a hosted large-language-model API. Treat feedback as practice guidance, not as a formal hiring assessment.

Session information may be stored in the browser's `localStorage`. Avoid using shared/public devices if you do not want another user of that browser profile to see locally stored session information. Clearing site data may erase it.

Google Fonts and Lucide are loaded from third-party CDNs, so an internet connection is needed for those external assets.

## Deploy with GitHub Pages

1. Push this repository to GitHub.
2. Open the repository's **Settings → Pages**.
3. Choose **Deploy from a branch**.
4. Select `main` and the root (`/`) folder, then save.
5. Wait for GitHub Pages to publish the site.

Because this is a static frontend, GitHub Pages can host it. Voice features still depend on browser support and permissions.

## Project files

- `index.html` — app structure and setup screens
- `style.css` — layout, responsive styles, and visual design
- `interview.js` — question database, session behavior, speech handling, and feedback logic

## Contributing

Fork the repository, create a branch for your change, test in a supported browser, and open a pull request.

## License

No license is included. Add a license file if you want to grant others explicit permission to use, modify, or redistribute this project.
