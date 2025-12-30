# Music Player Repository

## Overview
A web-based music player deployed to GitHub Pages that plays MP3 files from this repository.

## Live URL
https://sadensmol.github.io/music/

## Adding New Songs

When new music files are added to the repository, update the playlist in `index.html`:

1. Find the `musicFiles` array in the `<script>` section (around line 283)
2. Add the new filename to the array

Example:
```javascript
const musicFiles = [
    "თბილისის მზიანი სია.mp3",
    "Белый кот Беляш.mp3",
    "NEW_SONG.mp3",  // Add new songs here
];
```

To find all music files in the repo:
```bash
find . -type f \( -name "*.mp3" -o -name "*.wav" -o -name "*.ogg" -o -name "*.flac" -o -name "*.m4a" \) -not -path './.git/*'
```

## Features

- **Play button**: Click to play a track
- **Share button**: Copies a direct playback URL (e.g., `?play=0`) - opens page with only that track playing
- **Direct button**: Opens direct link to the MP3 file

## Deployment

Automatic deployment via GitHub Actions on push to `main` branch.

Workflow file: `.github/workflows/deploy.yml`

First-time setup:
1. Go to repository Settings > Pages
2. Set "Build and deployment" source to "GitHub Actions"
