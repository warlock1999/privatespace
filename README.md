##
- Tested image `https://github.com/sleeyax/stremio-streaming-server` in RunTipi since it was not available in the RunTipi Appstore.

- If you need to stream content online with HTTPS, you can add my App Store or create your own App Store and import the apps directory on your github App Store.

## Repository Structure

- **apps/**: Contains individual app directories

  - Each app has its own folder (e.g., `whoami/`) with the following structure:
    - `config.json`: App configuration file
    - `docker-compose.json`: Docker setup for the app
    - `metadata/`: Contains app visuals and descriptions
      - `description.md`: Markdown description of the app
      - `logo.jpg`: App logo image

- **tests/**: Contains test files for the app store

  - `apps.test.ts`: Test suite for validating apps

## Documentation

For detailed instructions on creating your own app store, please refer to the official guide:
[Create Your Own App Store Guide](https://runtipi.io/docs/guides/create-your-own-app-store)
