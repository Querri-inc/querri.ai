# Local Development Server Guide

This guide explains how to run your Querri website locally for testing purposes.

## Prerequisites

- Python 3.x installed on your computer
- Basic familiarity with terminal/command line

## Running the Server

1. Open a terminal window
2. Navigate to the directory containing your website files (where `server.py` is located)
3. Run one of the following commands:

### Basic usage

```bash
python server.py
```

This will start a server on port 8000. You can access your site at http://localhost:8000

### Specify a different port

```bash
python server.py -p 5000
```

This will start the server on port 5000. You can access your site at http://localhost:5000

### Specify a different directory to serve

```bash
python server.py -d /path/to/your/website/files
```

## Stopping the Server

To stop the server, press `Ctrl+C` in the terminal window where the server is running.

## Features

- Automatically serves `index.html` when accessing the root URL
- Includes CORS headers to allow testing from other origins
- Disables caching to ensure you always see the latest changes
- Simple and lightweight for quick testing

## Troubleshooting

- If you see "Address already in use" error, try using a different port with the `-p` option
- If you can't access the site, ensure there's no firewall blocking the port
- If changes don't appear, try hard-refreshing your browser (Ctrl+F5 or Cmd+Shift+R) 