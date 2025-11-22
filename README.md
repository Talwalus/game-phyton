# Miku Python Guessing Game

A small number-guessing game implemented with Brython (Python running in the browser).

## Requirements

- Python 3 (for serving the files locally)
- A modern browser (Chrome, Firefox, Edge, Safari) with JavaScript enabled

## Run locally

From the project root (where `index.html` lives) run a simple HTTP server:

```bash
python3 -m http.server 8000
```

Then open your browser to:

```
http://localhost:8000
```

Note: Some browsers block audio autoplay until the page receives user interaction. If you don't hear sounds, click anywhere on the page or press the Guess button once to enable audio playback.

## Quick tests

- Leave the input blank and click `Guess` → message should say `Enter a number!`.
- Type non-numeric text and click `Guess` → message should say `Invalid number!`.
- Type a number (or press Enter) and verify `Too low!`, `Too high!`, or `Correct!` responses and corresponding audio.

## Development notes

- The game uses Brython; the Brython runtime is loaded from CDN in `index.html`.
- Serve the files over HTTP rather than opening the file directly for best compatibility.

Enjoy! 🎵
