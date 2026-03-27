# Billboard Time Machine 🎵

A Python script that scrapes the Billboard Hot 100 chart for any given date and automatically creates a private Spotify playlist with the top songs — travel back in time through music!

## Features

- Scrapes the Billboard Hot 100 for any date you choose
- Searches for each song on Spotify
- Automatically creates a private playlist in your Spotify account
- Skips any songs that can't be found on Spotify

## Prerequisites

- Python 3.x
- A [Spotify Developer account](https://developer.spotify.com/dashboard) with an app created to obtain your `client_id` and `client_secret`

## Installation

1. Clone the repository:
```bash
   git clone https://github.com/your-username/billboard-time-machine.git
   cd billboard-time-machine
```

2. Install the required dependencies:
```bash
   pip install beautifulsoup4 requests spotipy
```

3. Replace the placeholders in the script with your Spotify credentials:
```python
   client_id=YOUR-CLIENT-ID,
   client_secret=YOUR-CLIENT-SECRET,
```

## Usage

Run the script and enter a date when prompted:
```bash
python main.py
```
```
Which year do you want to travel to? Type the date in this format YYYY-MM-DD:
```

A private playlist named `YYYY-MM-DD Billboard 100` will be created in your Spotify account.

## Notes

- On first run, you will be redirected to authenticate with Spotify. Your token will be cached in `token.txt` for future use.
- Songs not found on Spotify will be skipped and logged in the console.

