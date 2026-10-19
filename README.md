# Sentient Design listening companion

Steve’s original summaries of *Sentient Design* by Josh Clark with Veronika Kindred. Unofficial companion with AI-generated narration; not the book or its official audiobook.

Static HTML/CSS/JavaScript, no build step or backend. Serve this directory over HTTP (for example `python3 -m http.server 8000`). GitHub Pages serves the main branch root.

The player saves chapter positions, active chapter, speed and completed chapters in localStorage on the same browser/device. No cross-device sync. Storage clearing/private browsing can remove progress. Audio continues to the next available chapter after `ended`; browser autoplay restrictions are handled with a request to tap Play. Background playback and Media Session support depend on browser/OS.

To add or replace audio, copy an approved MP3 into `audio/` and edit `chapters.json`: stable numeric `id`, `title`, relative `src`, and `duration` in seconds. A null `src` shows a disabled coming-soon chapter. Do not put source books, generation receipts, credentials or private metadata into this repository.

Controls: play/pause, previous/next, ±15 seconds, seek, speed, reset progress, chapter selection, supported phone lock-screen actions. Space and arrow shortcuts apply outside interactive controls.
