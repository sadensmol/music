# Music

A simple music player web application that plays music files from this repository.

## Live Demo

**URL:** https://sadensmol.github.io/music/

## Getting Started

Once deployed, simply visit the URL above to:

1. See all music files in the playlist
2. Click on any track to play it
3. Use the audio controls to play/pause, seek, and adjust volume
4. Tracks auto-advance to the next song when finished

## Deployment

This project automatically deploys to GitHub Pages when you push to the `main` branch.

### First-time Setup

1. Go to your repository Settings
2. Navigate to **Pages** (under "Code and automation")
3. Under "Build and deployment", select **GitHub Actions** as the source
4. Push to `main` branch to trigger the deployment

## Adding Music

To add more music files:

1. Add your audio files (mp3, wav, ogg, etc.) to the repository
2. Update the `musicFiles` array in `index.html` with the new filenames
3. Commit and push to `main`
