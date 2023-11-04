# Spotify Integration Project

This project integrates with the Spotify Web API to enable users to log in with their Spotify account, search for tracks, and control playback through an Express web application.

## Features

- User authentication with Spotify
- Search for tracks using Spotify's search API
- Control playback of Spotify tracks

## Prerequisites

Before you begin, ensure you have met the following requirements:

- You have installed [Node.js](https://nodejs.org/en/) and npm (Node.js package manager).
- You have a Spotify Developer account and have set up an application to obtain the `CLIENT_ID` and `CLIENT_SECRET`.
- You have set up a `.env` file in your project root with your Spotify credentials and the correct `REDIRECT_URL`.

## Installation

To install the project, follow these steps:

1. Clone the repo:
   ```sh
   git clone https://github.com/adanzweig/nodejs-spotify.git
   ```
2. Navigate to the project directory:
   ```sh
   cd nodejs-spotify
   ```
3. Install the required dependencies:
   ```sh
   npm install
   ```

## Usage

To run the application, follow these steps:

1. Start the server:
   ```sh
   npm start
   ```
2. Open your web browser and navigate to:
   ```
   http://localhost:3050/login
   ```
3. Log in with your Spotify credentials.
4. You will be redirected to use the `/search` and `/play` endpoints to search for tracks and control playback.

## Endpoints

- `GET /login`: Redirects to Spotify's login page.
- `GET /callback`: Handles the callback after Spotify login.
- `GET /search`: Searches for tracks based on a query parameter `q`.
- `GET /play`: Starts playback of a track based on the provided URI query parameter.

## Contributing

To contribute to this project, follow these steps:

1. Fork the repository.
2. Create a new branch: `git checkout -b branch-name`.
3. Make your changes and commit them: `git commit -m 'commit message'`.
4. Push to the original branch: `git push origin branch-name`.
5. Create the pull request.

Alternatively, see the GitHub documentation on [creating a pull request](https://help.github.com/articles/creating-a-pull-request/).

## License

This project uses the following license: [MIT License](LICENSE).

## Acknowledgments

Thank you to the Spotify Web API and the creators of the `spotify-web-api-node` package for making this integration possible.