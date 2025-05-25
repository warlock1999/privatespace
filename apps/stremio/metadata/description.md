# Stremio

## Overview
Stremio is a modern media center that allows users to stream movies, TV shows, series, and other media content. It supports add-ons for accessing content from various sources and provides a user-friendly interface for organizing and watching media.

## Features
- Stream content from multiple sources via add-ons.
- Cross-platform support (Web, Desktop, Mobile).
- Personalized watchlists and recommendations.
- Supports local media playback and torrent streaming.

## Setup Instructions
1. Ensure Docker and Docker Compose are installed.
2. Place this folder in your `apps` directory.
3. Run `docker-compose up -d` in the `stremio/metadata` directory.
4. Access Stremio at `http://<your-server-ip>:11470`.

## Requirements
- Docker
- Internet connection for add-ons and streaming
- Persistent storage for user data

## Notes
- The Stremio server runs on port `11470`. Ensure this port is open if accessing remotely.
- Use the Stremio desktop or mobile app for the best experience, or access via the web interface.
- Add-ons can be installed through the Stremio interface for additional content sources.

## Links
- [Official Stremio Website](https://www.stremio.com/)
- [Stremio GitHub](https://github.com/Stremio/stremio-server)