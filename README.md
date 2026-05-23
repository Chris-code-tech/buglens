# BugLens 🔬

An AI-powered screenshot debugger built with Gemma 4. Upload a screenshot of any bug, error message, or broken UI — BugLens analyzes it and returns a structured diagnosis in seconds.

Built for the [Gemma 4 Challenge](https://dev.to/challenges/google-gemma-2026-05-06).

## What it does

Drop in any error screenshot and BugLens returns:

- **Error Type** — what kind of bug it is
- **Severity** — High / Medium / Low
- **Root Cause** — why it's happening
- **Affected Area** — what part of the code is involved
- **How to Fix** — step-by-step solution with code examples
- **Prevention** — how to avoid it in the future

## How it works

BugLens sends your screenshot directly to **Gemma 4 31B Dense** (`gemma-4-31b-it`) via the Google AI Studio API. The model reads the image, reasons about the error, and returns a structured analysis parsed into clean UI cards.

## Getting started

1. Clone the repo
2. Open `index.html` in your browser
3. Click ⚙️ and paste your [Google AI Studio API key](https://aistudio.google.com)
4. Upload a bug screenshot and hit **Analyze Bug**

No build step. No dependencies. Just one HTML file.

## Tech stack

- Vanilla HTML, CSS, JavaScript
- Gemma 4 31B Dense via Google AI Studio API

## License

MIT
