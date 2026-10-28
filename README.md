# Food Verse AI — Multimodal Food Intelligence Agent

A responsive multi-view frontend concept for exploring food intelligence. The dashboard presents a sample meal, estimated nutrition, ingredient recognition, meal-quality insights, a conversational assistant, hydration tracking, and a weekly summary.

> **Prototype notice:** This repository currently contains a static UI demo, not a connected multimodal AI agent. The meal analysis and weekly data are illustrative sample content. Chat answers are selected from local canned responses. Meal scanning, history, ingredient editing, and detailed nutrition controls show preview messages. Hydration updates only in the current page session and resets when the page reloads. Do not use the displayed nutrition values for medical or dietary decisions.

## Features in this demo

- Responsive dashboard layout for desktop and mobile screens
- Sample meal card with recognized ingredient labels
- Illustrative calorie, macronutrient, and meal-quality summaries
- Local demo chat with prompt chips and keyword-matched sample answers
- Session-only hydration counter, capped at the displayed daily goal
- Navigation feedback for sections that are not implemented yet
- Dynamic date display using the browser's local date

## Tech stack

- HTML5
- CSS3 (embedded in `index.html`)
- Vanilla JavaScript (embedded in `index.html`)
- Google Fonts and an Unsplash-hosted food image loaded from the web

No build system, package manager, server, or Python dependencies are required. `requirements.txt` is intentionally omitted because the project does not use Python. No API keys or environment variables are used, so `.env.example` is not needed.

## Run locally

1. Clone the repository:

   ```bash
   git clone https://github.com/YOUR-USERNAME/food-verse-ai.git
   cd food-verse-ai
   ```

2. Open `index.html` directly in a current browser, or use a simple local static server if you prefer:

   ```bash
   python -m http.server 8000
   ```

3. Visit `http://localhost:8000`.

The Google Fonts and Unsplash image need an internet connection. If they cannot load, the page remains usable with fallback fonts and a plain meal-image background color.

## Usage

- Review the pre-filled sample meal and its nutrition cards.
- Ask the demo assistant about protein, fiber, snacks, or vitamin C; it responds with local sample text.
- Select **Add a glass** to update the hydration figure for the current page session.
- Use **Scan a meal**, **View history**, **Edit ingredients**, and **Details** to see prototype preview messages.

## Screenshots

Add screenshots here before publishing, for example:

```markdown
![Food Verse AI dashboard](screenshots/dashboard.png)
```

Capture the page at desktop and mobile widths and save the images in a `screenshots/` directory.

## Project structure

```text
food-verse-ai/
├── index.html     # Complete static dashboard and interactions
├── README.md      # Project overview and setup guide
└── .gitignore     # Local secrets, environments, and generated files
```

## GitHub Pages

This is a static site and can be published with GitHub Pages from the repository root. In the repository settings, choose **Pages**, select the `main` branch and `/ (root)` as the source, then save.

## Roadmap

- Connect image upload/camera capture to a food recognition model
- Replace sample nutrition values with a sourced nutrition database
- Connect chat to a multimodal model through a secure backend
- Persist meals, user preferences, and hydration history
- Add validation, privacy controls, and tests for connected features

## License

No license is included yet. Add a license before accepting contributions or allowing reuse.

