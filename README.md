[![Global_hits](https://github.com/sahilkumardhala/Global-Hits/blob/main/Global_hits.png)](https://global-hits.vercel.app/)
# Global-Hits

Global-Hits is a lightweight single-page web app that showcases the most-viewed/viral songs from different languages and lets you play them using Play button in upper image.
---

## Table of Contents

- [Features](#features)
- [Demo](#demo)
- [Tech Stack](#tech-stack)
- [Files](#files)
- [Full Playlist (songData)](#full-playlist-songdata)
- [Installation](#installation)
- [Usage](#usage)
- [Customizing the playlist](#customizing-the-playlist)
- [Development Notes](#development-notes)
- [Contributing](#contributing)
- [Tests](#tests)
- [License](#license)
- [Contact](#contact)

---

## Features

- Curated list of popular songs across many languages
- Play/pause, next/previous track controls
- Seek scrubber with current time/duration display
- Volume control and mute/unmute
- Search songs by name or language
- Uses the YouTube IFrame Player API for playback

## Demo

Open `index.html` in your browser to run the app locally. The app uses the YouTube embed API, so an internet connection is required.

## Tech Stack

- HTML, CSS, JavaScript
- YouTube IFrame Player API (https://developers.google.com/youtube/iframe_api_reference)

## Files

- `index.html` — Main app file containing markup, styles, and embedded JavaScript (playlist data and player logic).
- `README.md` — This file.
- `LICENSE` — Project license (Apache 2.0).

## Full Playlist (songData)

Below is the full playlist extracted from `index.html`:

| # | Language | Song Name | Total Views | YouTube Video ID |
|---|---|---|---:|---|
| 1 | Chhattisgarhi | Maya Hoge Maya | 57 Million | eSfFKUjjv2Y |
| 2 | Doteli | Haai Haai Maya (Bambai Gaijane) | 71 Million | _mvve98Kb5Q |
| 3 | Garhwali | Dhana | 82 Million | 0hS7ti5PS5A |
| 4 | Rajasthani | Chaudhary | 138 Million | 1gukvtH_a3I |
| 5 | Polish | Ona by tak chciała | 235 Million | IP5jj0oNAWg |
| 6 | Nepali | Kutu Ma Kutu | 240 Million | VwIWfvW3SD8 |
| 7 | Sinhala | Manike Mage Hithe | 258 Million | PgCliOxl41o |
| 8 | Persian | Behet Ghol Midam | 284 Million | cDNDVtoJhik |
| 9 | Kannada | Karabu | 334 Million | LI8sVqjUSpE |
| 10 | Sanskrit | Shiva Tandava Stotram | 410 Million | w65nwf3GJ0c |
| 11 | Bengali | Oporadhi | 453 Million | PQDbJ-p0ivE |
| 12 | Telugu | Butta Bomma | 944 Million | 2mDCVzruYzQ |
| 13 | Bhojpuri | Hello Koun | 1.0 Billion | u43g_6a9780 |
| 14 | Russian | I Got Love | 1.1 Billion | nidQCt_8Pzk |
| 15 | German | Wind of Change | 1.2 Billion | n4RjJKxkeG4 |
| 16 | Arabic | Lm3allem | 1.2 Billion | _Fwf45pIAtM |
| 17 | Nigerian Pidgin | Calm Down | 1.4 Billion | WcIcVapfqXw |
| 18 | French | Dernière Danse | 1.4 Billion | K5KAc5CoCuk |
| 19 | Hindi | Vaaste | 1.7 Billion | BBAyRBTfsOU |
| 20 | Tamil | Rowdy Baby | 1.7 Billion | x6Q7c9RyMzk |
| 21 | Punjabi | Lehanga | 1.8 Billion | IEDEtZ4UVtE |
| 22 | Portuguese | Bum Bum Tam Tam | 1.9 Billion | _P7S2lKif-A |
| 23 | Korean | Gangnam Style | 5.9 Billion | 9bZkp7q19f0 |
| 24 | English | See You Again | 7.0 Billion | RgKAFK5djSk |
| 25 | Spanish | Despacito | 9.1 Billion | kJQP7kiw5Fk |



## Installation

1. Clone the repository:

   git clone https://github.com/sahilkumardhala/Global-Hits.git

2. Serve or open the project locally:

   - Double-click `index.html` to open in a browser.
   - For a local static server (recommended):
     - Python 3: `python -m http.server 8000`
     - Node (http-server): `npx http-server`


## Usage

- Use the search box to filter songs by name or language.
- Click any track in the list to load and play it.
- Use the play/pause button, previous/next buttons, and the seek bar to control playback.
- Use the volume slider or mute button to control audio.

## Customizing the playlist

The song list is stored in a JavaScript array inside `index.html` named `songData`. Each entry has the shape:

```js
{ "language": "English", "song_name": "See You Again", "total_views": "7.0 Billion", "video_id": "RgKAFK5djSk" }
```

To add, remove, or modify tracks, edit the `songData` array. The app automatically re-renders the playlist on page load.

Note: video playback depends on YouTube embeds and the provided `video_id` values.

## Development notes

- The app is intentionally dependency-free (no build step). If you plan to extend it, consider splitting the CSS and JS into separate files and using a build tool.
- For debugging the YouTube API, open the browser console to inspect player events and errors.
- If you plan to publish or deploy this project, ensure the YouTube usage complies with YouTube Terms of Service.

## Contributing

Contributions are welcome. Suggested process:

1. Fork the repository
2. Create a branch for your change: `git checkout -b feature/my-change`
3. Make changes and test locally
4. Open a pull request describing your changes

Please keep changes focused and include a short description of why the change is needed.

## Tests

There are no automated tests included. If you add tests, document how to run them here.

## License

This project is licensed under the Apache License 2.0. See the `LICENSE` file for details.

## Contact

Repository owner: @sahilkumardhala

If you want additional edits (badges, screenshots, demo link, or split files), tell me what to include and I will update the README accordingly.

![play back](https://github.com/sahilkumardhala/Global-Hits/blob/main/play_list.png)
