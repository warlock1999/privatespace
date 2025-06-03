# Shoko Server

Shoko Server is an open-source, cross-platform anime management system designed to automate and streamline the organization of your anime collection. It integrates with AniDB to hash and match your files against a comprehensive database, ensuring accurate series and episode identification. Shoko supports multiple media players like Plex, Jellyfin, and Kodi, allowing you to access your collection locally or remotely with ease. With features like automatic metadata retrieval, watch state synchronization, and file management, Shoko eliminates the need for manual organization, letting you focus on enjoying your anime.

## Features
- **Automated Cataloging**: Hashes files and matches them with AniDB for precise series and episode identification.
- **Metadata Integration**: Pulls detailed metadata and images from AniDB, TMDB, and other sources for a rich collection experience.
- **Media Player Support**: Seamlessly integrates with Plex, Jellyfin, and Kodi for flexible streaming and playback.
- **Watch State Syncing**: Tracks and syncs watch progress across supported platforms like Trakt and Plex.
- **File Management**: Automatically renames, moves, and organizes files using metadata and custom plugins.
- **Scalability**: Handles collections of any size, from small libraries to extensive archives.
- **Web UI**: User-friendly interface for managing your collection, accessible via browser at `http://localhost:8111`.

## Setup Instructions
1. **Install Shoko Server**: Download the latest version from [shokoanime.com](https://shokoanime.com) and follow the installation guide for your platform (Windows, Linux, or Docker).
2. **Configure AniDB Account**: Create or link an AniDB account in the Shoko Web UI to enable file hashing and metadata retrieval.
3. **Add Import Folders**: Specify the physical locations of your anime files in the Web UI for Shoko to scan and organize.
4. **Integrate with Media Players**: Install plugins like Shoko Metadata for Plex or Shokofin for Jellyfin to enhance integration.
5. **Customize Settings**: Adjust metadata sources, watch state syncing, and file renaming preferences in the Web UI.

## Notes
- Shoko Server requires an AniDB account for core functionality. Ensure your credentials are correctly configured to avoid import issues.
- For remote access, consider using a VPN or reverse proxy (e.g., NGINX) for security, as direct internet exposure is not recommended.
- Regularly check for updates to ensure compatibility with the latest media players and metadata sources.

For more details, visit the [Shoko Documentation](https://docs.shokoanime.com) or join the [Shoko Discord](https://discord.gg/vpeHDsg) for community support.

*© 2016-2025 Shoko. All rights reserved. Images and related content are used for reference and non-commercial purposes.*