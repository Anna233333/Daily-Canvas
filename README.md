# Daily Canvas

Daily Canvas is a private, browser-based pointillist mood journal. Write one sentence, choose **Paint**, and the app turns that moment into one colored paint dot. Every entry in a month joins the same evolving pointillist composition while retaining its original date.

**Live site:** <https://anna233333.github.io/Daily-Canvas/>

## Run it

No build step or dependencies are required.

1. Open `code/index.html` in a modern browser, or serve the project locally:

   ```sh
   cd code
   python3 -m http.server 8000
   ```

2. Visit `http://localhost:8000`.

Entries are stored in the browser's local storage and do not leave the device.

## Project structure

```text
Daily Canvas/
├── README.md
├── .gitignore
├── code/
│   ├── index.html
│   ├── styles.css
│   └── app.js
├── docs/
│   ├── Design.md
│   └── learning-notes.md
└── tests/
    └── manual-test-plan.md
```

## Features

- One sentence creates exactly one impressionist-style dot.
- Transparent keyword analysis suggests a built-in or custom mood color.
- Suggested colors can be changed before painting.
- Add personal mood words or phrases and assign custom colors.
- Recolor the built-in mood palette; preferences persist locally.
- One combined pointillist canvas per month, with a calendar for choosing entry dates.
- Deterministic dot placement: paintings remain stable after refresh.
- Local persistence, inline editing, deletion with a three-second undo, keyboard support, and reduced-motion support.

## Privacy

Daily Canvas is intentionally local-first. Clearing browser storage removes saved entries. It is a reflective art tool, not a diagnostic or mental-health assessment.
