# Guitar Note Recognition Exercise

A single-file, client-side web app for practicing rapid note recognition on guitar.  
Hit **Play**, listen to the spoken note (with string), and play it. As you improve, speed up the rate.

> If you're having any issues on **iOS / Safari**, see the notes below.

---

## Features

- 🎵 Text-to-speech calls out notes (e.g., “A flat on D string”)
- ♯/♭ awareness: `#`/`♯` → “sharp”, `b`/`♭` → “flat”
- 🔁 Optional “speak each note twice”
- 🎲 Randomized order (toggleable)
- ⏱️ Adjustable “rate of notes” (seconds between); handy –0.5 / +0.5 buttons
- 🗂️ Full default list (all six strings, frets 0–12) prepopulated and saved locally
- 🗣️ Pick any installed voice available to your browser
- ⌨️ Shortcuts: **S** start, **P** pause, **R** resume, **X** stop
- 📱 Mobile-friendly layout + sticky Start/Stop header

---

## Quick Start (Local)

1. Open `index.html` in a modern browser (Chrome, Edge, Safari, Firefox).
2. Click **Start** (some browsers require a user interaction to allow speech).
3. Adjust the **Rate of notes (seconds between)** as you progress.

Your custom list is saved automatically in your browser via `localStorage`.


---

## Safari / iOS Notes

- Tap **Start** once to allow audio (Safari blocks speech until user interaction).
- If silent: check device mute switch / Focus modes.  
  On macOS Safari: **Settings → Websites → Auto-Play** → **Allow All Auto-Play**.
- If the first note is skipped, tap **Start** again.
- Give the voice list a moment to load, or choose another voice if it sounds odd.

---

## Customization

- **Voices:** Choose from the dropdown (depends on OS/browser).
- **Randomization:** Toggle **Always randomized**.
- **Regenerate list:** Use the button to create a fresh randomized full set.
- **Edit list:** One phrase per line, e.g.  
  `F# on E string`  
  `Bb on A string`

> Pronunciation is auto-formatted: `F#` → “F sharp”, `Bb` → “B flat”, etc.  
> Leading “A” is read as the letter (so “Ab” becomes “A. flat”) to avoid article “uh”.

---

## Keyboard Shortcuts

- **S** – Start
- **P** – Pause
- **R** – Resume
- **X** – Stop

---

## Privacy

- No tracking, no analytics, no network calls.
- Your list is stored locally in your browser’s `localStorage`.

---

## Tech Notes

- Single static file (`index.html`)
- Uses the Web Speech API (`speechSynthesis`)
- Works offline once loaded (pure client-side)

---

## Credits

Based on a practice concept from the book **_Vaideology_** by **Steve Vai**.

