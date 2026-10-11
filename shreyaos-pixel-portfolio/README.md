# ShreyaOS — Pixel-Art Portfolio 🌷

A pastel, retro pixel-art portfolio that turns a browser window into a playful macOS-inspired desktop. Click project icons to open draggable windows, explore the portfolio, and find the **Rejected Concepts** Easter egg.

Live Website: 
https://shreyasharmaosportfolio.netlify.app

## Features

- Pastel pink, peach, and lavender desktop with floating clouds
- macOS-inspired menu bar and live clock
- Sticky-note introduction and custom inline SVG pixel character
- Project-specific desktop icons and interactive project windows
- Draggable, stackable windows with close, minimize, and maximize controls
- Boot-up intro and 8-bit-style sounds generated in the browser
- Sound on/off toggle and Rejected Concepts trash-can Easter egg
- Responsive styling for smaller screens

## Contact details

The portfolio Contact window includes an email link for `shreyasharma3521@gmail.com`, plus GitHub and LinkedIn links. The email link opens the visitor’s default email app; it does not connect to or expose the Gmail inbox.

## Technology stack

| Technology | Use in this project |
|---|---|
| HTML5 | Desktop structure, icons, project windows, content, and inline SVG |
| CSS3 | Layout, pastel gradients, window styling, responsive rules, and animations |
| Vanilla JavaScript (ES6+) | Clock, window controls, dragging, boot sequence, and interactions |
| SVG | Pixel-art character illustration embedded in HTML |
| Web Audio API | Generates short retro sound effects in the browser |
| Google Fonts | Press Start 2P and VT323 typography |
| Git and GitHub | Version control and repository hosting |

This is a **static frontend project**. It does not currently use React, Node.js, a database, or a backend API. No package installation or build step is required.

## Project structure

```text
shreyaos-pixel-portfolio/
├── index.html          # HTML structure and portfolio content
├── css/
│   └── style.css       # All page styling and responsive design
├── js/
│   └── script.js       # Clock, windows, sound, boot screen, interactions
├── .gitignore
└── README.md
```

## Run locally in VS Code

1. Download and extract this repository, or clone it from GitHub.
2. In VS Code, choose **File → Open Folder** and select `shreyaos-pixel-portfolio`.
3. Keep the folders and filenames exactly as shown above; the HTML links to `css/style.css` and `js/script.js`.
4. Install the **Live Server** extension in VS Code if you do not already have it.
5. Right-click `index.html` and select **Open with Live Server**.
6. Click **BOOT UP** and explore the desktop icons.

Alternatively, if Python is installed, open a terminal in the project folder and run:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000> in your browser. You can also open `index.html` directly, but a local server is recommended for development.

## How the files work together

- `index.html` defines the content and loads the other files using `<link rel="stylesheet" href="css/style.css">` and `<script src="js/script.js" defer></script>`.
- `css/style.css` controls the visual design. Change colors, sizes, spacing, and animations here.
- `js/script.js` controls interactivity. The Web Audio API is a browser feature called by JavaScript, so it does not need its own file. Google Fonts are loaded through a stylesheet link in `index.html`, so font files are not stored in this repository.

## Personalize before publishing

- The Contact window includes `shreyasharma3521@gmail.com` with an email link and a copy-email button. Update the address in both `index.html` and `js/script.js` if it changes.
- Verify your LinkedIn profile URL in `index.html`.
- Update GitHub links to point to the individual project repositories when available.
- Review project descriptions, skills, and contributions for accuracy.
- Edit the sticky-note tagline and portfolio content in `index.html`.

The fonts are loaded from Google Fonts, so an internet connection is needed to load Press Start 2P and VT323. Fallback fonts will be used if the service is unavailable. Sound may require a user click because of browser autoplay restrictions.

## Deploy with GitHub Pages

1. Create a GitHub repository named `shreyaos-pixel-portfolio`.
2. Upload the complete project structure, including the `css` and `js` folders (not just `index.html`).
3. Open **Settings → Pages** in the repository.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/(root)` folder, then save.
6. Wait for GitHub Pages to publish the website; the live URL will appear in the Pages settings.

## Notes

- This is a portfolio demo, not a full operating-system emulator.
- The inline SVG character is part of `index.html`; it does not need a separate image file.
- Clipboard access may require HTTPS or localhost.

## License

No license is currently included. Add one if you want to specify how others may reuse the project.
