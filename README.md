# Global-Hits

Global-Hits is a lightweight single-page web app that showcases the most-viewed/viral songs from different languages and lets you play them using the YouTube IFrame Player API. It’s built with vanilla HTML, CSS, and JavaScript and is designed to be simple to run and customize.

## Features

- Curated list of popular songs across many languages
- Play/pause, next/previous track controls
- Seek scrubber with current time/duration display
- Volume control and mute/unmute
- Search songs by name or language
- Uses the YouTube IFrame Player API for playback

## Demo

Open `index.html` in your browser to run the app locally. The app uses the YouTube embed API, so an internet connection is required.

## Tech stack

- HTML, CSS, JavaScript
- YouTube IFrame Player API (https://developers.google.com/youtube/iframe_api_reference)

## Files

- `index.html` — Main app file containing markup, styles, and embedded JavaScript (playlist data and player logic).
- `README.md` — This file.
- `LICENSE` — Project license.

## Usage

1. Clone the repository:

   git clone https://github.com/sahilkumardhala/Global-Hits.git

2. Open the app in a browser:

   - Double-click `index.html` or serve the directory using a static server (recommended for some browser environments):
     - Python 3: `python -m http.server 8000`
     - Node (http-server): `npx http-server`

3. Use the UI to search and play tracks. Controls are self-explanatory: play/pause, next, previous, seek bar, and volume.

## Customizing the playlist

The song list is stored in a JavaScript array inside `index.html` named `songData`. Each entry has the shape:

```js
{ "language": "English", "song_name": "See You Again", "total_views": "7.0 Billion", "video_id": "RgKAFK5djSk" }
```

To add, remove, or modify tracks, edit the `songData` array. The app automatically re-renders the playlist on page load.

Note: video playback depends on YouTube embeds and the provided `video_id` values.

## Development notes

- The app is intentionally dependency-free (no build step). If you plan to extend it, you can split the JS/CSS into separate files.
- For debugging the YouTube API, open the browser console to inspect player events and errors.

## Contributing

Contributions are welcome. Suggested process:

1. Fork the repository
2. Create a branch for your change: `git checkout -b feature/my-change`
3. Make changes and test locally
4. Open a pull request describing your changes

Please keep changes focused and include a short description of why the change is needed.

## License

This repository includes a `LICENSE` file. Please refer to it for license details.

## Contact

Repository owner: @sahilkumardhala

If you want changes to the README content (add screenshots, demo link, badges, or more project-specific instructions), tell me what to include and I’ll update the file.
