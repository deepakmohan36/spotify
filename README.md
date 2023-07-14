# Spotify Artist Songs

This repository contains Python code that interacts with the Spotify API to search for an artist and retrieve their top songs. It utilizes the `dotenv` library to load environment variables for authentication with the Spotify API.

## Prerequisites

Before running the code, make sure you have the following:

- Python 3.x installed on your system
- Spotify API credentials (client ID and client secret)
- Spotify developer account (to obtain API credentials)

## Installation

1. Clone the repository to your local machine:

   ```
   git clone https://github.com/your-username/spotify-artist-songs.git
   ```

2. Install the required dependencies by running the following command:

   ```
   pip install -r requirements.txt
   ```

3. Create a `.env` file in the project root directory and add your Spotify API credentials:

   ```plaintext
   client_id=<your-client-id>
   client_secret=<your-client-secret>
   ```

## Usage

Run the Python script to search for an artist and retrieve their top songs:

```bash
python spotify_artist_songs.py
```

Make sure you have set up the `client_id` and `client_secret` environment variables correctly in the `.env` file.

## Code Explanation

The code in `spotify_artist_songs.py` does the following:

1. Loads the `dotenv` library and imports necessary modules.

2. Retrieves the Spotify API credentials from the environment variables.

3. Defines a function `get_token()` to obtain an access token from the Spotify API using client credentials.

4. Defines a function `get_auth_header(token)` to generate the authorization header for API requests.

5. Defines a function `search_for_artist(token, artist_name)` to search for an artist by name and retrieve their information.

6. Defines a function `songs_by_artist(token, artist_id)` to retrieve the top songs of an artist given their Spotify ID.

7. Calls the necessary functions to search for an artist and retrieve their top songs.

8. Prints the top songs of the artist to the console.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or create a pull request in this repository.

