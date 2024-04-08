# YouTube Video Fetcher Project -  Raghav Tiwari

Welcome to the Fampay YouTube Video Fetcher! This is a Flask application that fetches the latest videos from YouTube for a given tag/search query in a paginated response. It's designed to be scalable and reliable, making it perfect for projects of all sizes.

## Table of Contents

- Project Goal
- Features
- Requirements
- Setup
- Usage
- Contributing
- License

## Project Goal

The goal of this project is to create an API that fetches the latest videos sorted in reverse chronological order of their publishing date-time from YouTube for a given tag/search query in a paginated response. This is achieved by continuously calling the YouTube API in the background at a specified interval (e.g., every 10 seconds) and storing the video data in a database.

## Features

- Fetches the latest videos from YouTube for a given tag/search query
- Stores video data in a SQLite database
- Provides a paginated API to fetch the video data
- Runs the video fetching task in the background

## Requirements

- Python 3.6+
- Flask
- SQLAlchemy
- Requests

## Setup

1. Clone the repository:
    ```
    git clone https://github.com/raghavtiwari07/fampay.git
    cd fampay
    ```

2. Install the requirements:
    ```
    pip install -r requirements.txt
    ```

3. Set the environment variables:
    ```
    export FLASK_APP=run.py
    export YOUTUBE_API_KEY=your-youtube-api-key
    ```

4. Run the application:
    ```
    flask run
    ```

## Usage

To get the videos, send a GET request to `/videos` with an optional `page` parameter. For example:
http://localhost:5000/videos?page=2

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. Please make sure to update tests as appropriate.

Please replace your-youtube-api-key with your actual YouTube API key. 
Also, remember to add a requirements.txt file with all the dependencies of your project.
You can generate it using pip freeze > requirements.txt.


