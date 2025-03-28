---
title: "Rudi Mental"
image: "rudi_interface.png"
badges:
  - name: "Live Demo"
    url: "https://stalinon.github.io/rudi-mental/"
  - name: "GitHub"
    url: "https://github.com/stalinon/rudi-mental"
---

**Rudi Mental** is a web application for drummers that combines a metronome with a rudiment training tool. It plays rhythm patterns with visual beat indicators, supports tempo, time signature, and exercise customization, and includes "sound/silence" cycle modes. It features real-time note rendering via ~~**VexFlow**~~ **ABCJS**, accent control, and interactive metronome behavior.

The app is built with React, using **Tone.js** for metronome sound generation, **MUI** for UI components, and ~~**VexFlow**~~ **ABCJS** for musical notation rendering.

---

## Plan

| Status   | Priority  | Task                                                                                   |
|----------|-----------|----------------------------------------------------------------------------------------|
| ✅ Done   | High      | ~~Basic metronome implementation~~                                                         |
| ✅ Done   | Medium    | ~~Cycle of "sound bars — silent bars" for internal timing training~~                       |
| ✅ Done   | Medium    | ~~Light/dark theme toggle~~                                                                |
| ✅ Done   | Medium    | ~~Displaying notation for exercises~~                                                      |
| ✅ Done | High      | ~~Switch to SVG notation from Groove Scribe~~                                              |
| ✅ Done | Medium    | ~~Allow users to add their own exercises via links (stored in localStorage)~~              |
| ✅ Done | Low       | ~~Shared storage of exercises (e.g., via Google Sheets API without backend)~~              |
| ✅ Done | Medium    | ~~Highlight quarter notes in sync with metronome~~                                         |
| 🛠️ To Do | Medium    | Expand exercise library                                                                |
| 🛠️ To Do | Low     | Progressive training: tempo increase, time signature changes                          |
| 🕗 Backlog | Medium  | Categorization/tagging of exercises                                                    |
| 🕗 Backlog | Medium  | Auto-evaluation of timing using mic or MIDI                                            |
| 🕗 Backlog | Medium  | Export of exercises as PDF                                                             |
| 🕗 Backlog | Low     | MIDI controller support                                                                |
| 🕗 Backlog | Low     | Training progress chart/visualization                                                  |
| 🕗 Backlog | Low     | Visual tempo representation through color                                              |
| 🕗 Backlog | Low     | Import/export presets via JSON/links                                                   |
| 🕗 Backlog | Low     | Offline support (PWA mode)                                                              |

---
