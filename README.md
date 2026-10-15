# Cadence — Songwriter’s Sketch Studio

An offline-first songwriting sandbox. Turn a mood into a chord progression, shape the voicing and tone, hear it through a browser synth, and watch the live audio signal split through a responsive prism visualization. No account, API key, paid service, build step, or backend is required.

## What works

### Studio and composition
1. Mood-to-progression composition using local music-theory templates.
2. Twelve root keys.
3. Major, natural minor, Dorian, Mixolydian, and major pentatonic scales.
4. Four, six, or eight-chord arrangements.
5. Triad, seventh, and rich-extension voicings.
6. Smooth voice-leading option.
7. One-click alternate takes.
8. Mood presets for twelve writing prompts.
9. Individual chord audition.
10. Keyboard shortcuts for playback, new takes, saving, tempo, and chord audition.
11. Undo and redo for progression edits.
12. Chord insertion from the Harmony Lab.
13. Transpose by one or two semitones.
14. Current key, scale, Roman numeral, and chord-tone chart.

### Audio and visualization
15. Browser-based Web Audio synth; first playback starts audio after user interaction.
16. Five selectable synth voices: soft keys, tape piano, glass bell, warm organ, and muted pluck.
17. Adjustable tempo from 40 to 220 BPM.
18. Tap tempo.
19. Loop or stop-after-one-take playback.
20. Metronome click.
21. Adjustable chord hold.
22. Swing timing.
23. Optional bass line.
24. Optional soft-strum layer.
25. Adjustable room reverb.
26. Adjustable echo.
27. Master volume.
28. Live analyser-driven prism dispersion, scope, and spectrum views.
29. Animated cassette reels and take-position indicator.
30. Scale-aware clickable piano keyboard.

### Projects, sharing, and learning
31. Local take library with search and sorting.
32. Save, reopen, and delete takes on this device.
33. JSON project export and import.
34. MIDI export for the current progression.
35. WAV render/export using the browser’s offline audio renderer.
36. Copy chord chart to clipboard.
37. Shareable URL containing a compact take snapshot.
38. Interactive circle of fifths to explore related keys.
39. Chord explorer with major, minor, suspended, diminished, augmented, seventh, and add-nine colors.
40. Harmony notes explaining progression choices.
41. Responsive mobile layout and reduced-motion support.
42. Local-only data model; no prompts or saved takes are sent to a server.

## Run locally

Open `index.html` in a modern browser. For best module and file-import compatibility, serve the folder with any static server, for example:

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Deploy to Vercel

Import the folder or repository as a static site. Use no framework, no build command, and `.` as the output directory. The included files are plain HTML, CSS, and JavaScript.

## Notes

- Saved takes are stored in the browser’s local storage and are device/browser-specific until exported.
- Audio is synthesized for sketching and is not a sample library or a finished production instrument.
- WAV export uses an offline render of the current chord arrangement; live visualization reflects the real-time Web Audio signal.
- Google Fonts are an optional network enhancement. The site falls back to local system fonts when offline.
