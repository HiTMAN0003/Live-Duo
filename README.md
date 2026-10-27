# Live Duo

A lightweight static YouTube Live dashboard for watching two streams and their live chats side by side.

## Deploy to GitHub Pages

1. Upload the files in this folder to the root of your GitHub repository.
2. Open **Settings → Pages**.
3. Under **Build and deployment**, choose **GitHub Actions**.
4. Push to `main`. The included workflow publishes the static site.

## Features

- Two YouTube live streams and chats in one layout.
- Hide video playback and keep the live chat visible.
- Optional viewer and like counts using a YouTube Data API v3 key.
- Saves stream IDs, video visibility, and API key in this browser's local storage.
- Responsive mobile drawer and dark theme.

## Counts and API quota

Viewer and like counts require a YouTube Data API v3 key with the YouTube Data API enabled in Google Cloud. The page refreshes counts every 60 seconds while open. The key is saved only in this browser's local storage, but it is still exposed to the browser; restrict it to the YouTube Data API and your deployed site's HTTP referrers in Google Cloud. Video and chat embeds work without the key.

## Notes

GitHub Pages serves static files only. YouTube's own embed restrictions still apply, and some videos may not allow embedding or live chat embeds.
