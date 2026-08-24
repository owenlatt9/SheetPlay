# SheetPlay

A simple local practice tool for musicians. Load your own sheet music PDF and audio track, set a metronome count-in, and play along — all in one HTML file, no install required.

## Why

Most tab/sheet-music apps only work with their own catalog. SheetPlay lets you use **your own files** — a PDF you already have and any audio file on your computer — with a metronome count-in and a bar/beat counter so you always know where you are in the piece.

## Features

- **PDF viewer** — load or drag-and-drop your sheet music, flip pages, zoom, and scroll
- **Your own audio** — load any audio file (MP3, WAV, AAC, FLAC, etc.) from your computer
- **Metronome count-in** — set BPM, time signature, and how many bars to count in before the track starts
- **Beat ticker** — visual dots show the beat live, with the bar number displayed large on screen
- **Waveform scrubbing** — click anywhere on the waveform to jump to that point in the track
- **Adjustable start point** — line up exactly where the count-in hands off to the recording, with an option to hear the track's intro playing under the count-in
- **Presets** — save your PDF, audio, tempo, and settings together and reload them later
- **Resizable, collapsible layout** — arrange the panel the way you like it

## Getting Started

1. Download `sheetplay.html`
2. Double-click it (or open it in Chrome/Safari)
3. Load a PDF and an audio file
4. Set your BPM, time signature, and count-in length
5. Hit play (or press `Space`)

No build step, no server, no dependencies to install — it's a single HTML file.

> **Note:** Presets are saved in your browser's local storage. This works most reliably in **Chrome**. Safari sometimes blocks local storage when opening a file directly (`file://`), so presets may not save there.

## Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `Space` | Play / Pause |
| `R` | Stop and reset |
| `←` / `→` | Previous / next PDF page |
| `↑` / `↓` | Increase / decrease BPM |

## Tech

Plain HTML, CSS, and JavaScript. Uses [PDF.js](https://mozilla.github.io/pdf.js/) for rendering sheet music and the Web Audio API for the metronome click. Everything runs client-side in the browser — your files never leave your computer.

## Roadmap Ideas

- Tap-tempo detection for setting BPM and start point by ear
- Setlists (queue multiple pieces/presets in order)
- Loop sections for practicing tricky parts

## License

Personal project — use it, fork it, modify it for your own practice setup.
