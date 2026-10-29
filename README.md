# LoopCount

A lightweight, responsive audio player that repeats your own audio files **11, 21, 51, or 108 times**, shows the number of fully completed repetitions, and stops automatically when the target is reached.

## Features

- Select an audio file directly from your device. Your audio **is not uploaded to a server**.
- Preset targets: 11, 21, 51, and 108 complete plays.
- Live progress bar, complete-play counter, pause/play, and reset controls.
- Standard audio element for native playback controls.
- Built-in alternative file loading method and troubleshooting panel.
- Works as a static site: no dependencies, accounts, build tools, or backend.

## Publish on GitHub Pages

1. Create a **public** GitHub repository, e.g. `loopcount`.
2. Upload `index.html`, `.nojekyll`, and `README.md` at the repository root (or push them via Git).
3. Open **Settings → Pages → Build and deployment**.
4. Set **Source** to **Deploy from a branch**, select your main branch and **/(root)**, then **Save**.
5. After deployment completes, visit `https://YOUR-USERNAME.github.io/loopcount/`.

You may share this link with friends. Everyone selects their **own local audio file**; no audio files are included with the site or stored by it.

## Supported devices and limitations

Works in modern browsers supporting HTML5 audio and file selection (Chrome, Safari, Firefox, Edge; Android, iOS, Windows, macOS, Linux). Actual playback depends on the device's audio decoding and browser media policies.

- Click/tap **Play** to start; browsers block unsolicited autoplay.
- On some mobile devices, switching apps or locking the screen may interrupt playback or prevent the next automatic repeat.
- Keep the tab active for the most reliable repetition count, especially on mobile.
- Files over 25 MB use a local blob URL rather than an in-memory data URL.

## Privacy

All processing is performed locally in the browser. The selected audio file is not sent to GitHub or the website server. (As with any hosted web page, visiting the page still involves a normal HTTP request for the HTML file.)

## Development

Open `index.html` directly or serve this directory with any static HTTP server. There are no external packages.

## Repository description

A lightweight, browser-based audio player that loops your audio files with automatic repetition counting and customizable repeat limits.