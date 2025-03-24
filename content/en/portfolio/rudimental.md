---
title: "Rudi Mental"
image: "rudi_interface.png"
badges:
  - name: "Live Demo"
    url: "https://stalinon.github.io/rudi-mental/"
  - name: "GitHub"
    url: "https://github.com/stalinon/rudi-mental"
---

**Rudi Mental** is a web application for drummers that combines a metronome with a rudiment training tool. It plays rhythm patterns with visual beat indicators, supports tempo, time signature, and exercise customization, and includes "sound/silence" cycle modes. It features real-time note rendering via **VexFlow**, accent control, and interactive metronome behavior.

The app is built with React, using **Tone.js** for metronome sound generation, **MUI** for UI components, and **VexFlow** for musical notation rendering.

---

## Key Features

### Visual Metronome
- Animated beat and bar indicators
- Accent recognition (strong first beat)
- Adjustable tempo from 20 to 240 BPM

### Exercise Mode
- Import exercises from JSON
- Displays three bars (previous / current / next)
- Supports R/L hand notation, rests, and accents
- Auto-stop at the end of the exercise

### Time Signature & Cycle Settings
- Custom time signatures (e.g., 3/4, 5/4, 6/8, etc.)
- Sound/silence bar alternation (for focused practice)
- Customizable number of "playing" and "mute" bars

---

## Architecture

The app is built with a modular React component structure:

- **MetronomeButton.jsx** — start/stop controller with BPM display
- **BeatVisualizer.jsx** — interval-based click engine via **Tone.js**
- **NoteViewer.jsx** + **BarRendererVex.jsx** — renders bars with accents and R/L annotations
- **TempoSlider.jsx** — interactive BPM slider
- **Modal components** — for rhythm, exercise, and metronome configuration

---

## Tech Stack

**Frontend:**
- React
- MUI (Material UI)
- VexFlow (notation rendering)
- Tone.js (metronome sound)
- JavaScript

**Infrastructure:**
- JSON-based exercises in `public/exercises/`
- Zero-backend: everything runs client-side

**Development & Deployment:**
- CRA (Create React App)
- GitHub Pages

---

## Exercise Format Example

```json
{
  "timeSignature": { "top": 4, "bottom": 4 },
  "bars": [
    [{ "hand": "R", "hit": true, "duration": "4" }, ...]
  ]
}
