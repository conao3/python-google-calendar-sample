# python-google-calendar-sample

A Python sample application demonstrating how to interact with the Google Calendar API.

## Overview

This project provides a command-line interface to fetch and display upcoming events from your Google Calendar. It's based on the official [Google Calendar API quickstart](https://developers.google.com/calendar/quickstart/python) with additional CLI enhancements using Click.

## Requirements

- Python 3.8+
- Google Cloud project with Calendar API enabled
- OAuth 2.0 credentials (`credentials.json`)

## Installation

1. Clone the repository:

```bash
git clone https://github.com/conao3/python-google-calendar-sample.git
cd python-google-calendar-sample
```

2. Install dependencies using Pipenv:

```bash
pip install pipenv
pipenv sync
```

3. Set up Google Cloud credentials:
   - Go to the [Google Cloud Console](https://console.cloud.google.com/)
   - Create a new project or select an existing one
   - Enable the Google Calendar API
   - Create OAuth 2.0 credentials and download as `credentials.json`
   - Place `credentials.json` in the project root

## Usage

Run the application to fetch your next 10 calendar events:

```bash
pipenv run python main.py fetch
```

On the first run, a browser window will open for OAuth authentication. Your credentials will be cached in `token.pickle` for subsequent runs.

## License

MIT License - See [LICENSE](LICENSE) for details.

## Author

Naoya Yamashita ([@conao3](https://github.com/conao3))
