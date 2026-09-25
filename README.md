# Daily Canvas

Daily Canvas is a private, browser-based pointillist mood journal. Write one sentence, choose **Paint**, and the app turns that moment into one paint dot. A sentence with several recognized feelings becomes one soft, multicolor dot, while every entry in a month joins the same evolving pointillist composition and retains its original date.

## Links

- **GitHub repository:** <https://github.com/Anna233333/Daily-Canvas>
- **Live website:** <https://anna233333.github.io/Daily-Canvas/>

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
- Transparent keyword analysis suggests built-in or custom mood colors.
- Multiple feelings produce one score-weighted gradient dot; stronger or repeated feelings receive more space while every recognized mood stays visible.
- Suggested colors can be overridden with one solid palette color before painting.
- Add personal mood words or phrases and assign custom colors.
- Recolor the built-in mood palette; preferences persist locally.
- One combined pointillist canvas per month, with a calendar for choosing entry dates.
- Deterministic dot placement: paintings remain stable after refresh.
- Local persistence, inline editing, deletion with a three-second undo, keyboard support, and reduced-motion support.

Neutral is used only when no non-neutral feeling is recognized. Mixed labels such as **Joy + Anxiety + Tiredness** remain visible in the moment list and accessible dot descriptions, so color is never the only signal. Editing an entry's words preserves its original paint, date, and position.

## Privacy

Daily Canvas is intentionally local-first. Clearing browser storage removes saved entries. It is a reflective art tool, not a diagnostic or mental-health assessment.
