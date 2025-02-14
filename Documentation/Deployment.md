# Deployment

## Requirements
- **Vue.js**: Required for running the frontend components.
- **Python**: Install Python (version 3 or above).

## Folder Structure and File Placement
1. **Frontend**
   Navigate to `Frontend` as the main application directory.
   Important files:
     - `package.json` - Defines dependencies and scripts for Node.js.
     - `src` - Contains main source code files.
     - `public` - Contains assets to be accesssed by the frontend.

2. **Backend**
   The `Backend` folder contains files which handle backend data processing tasks.
   Important files:
   - `stock_info.py` - API calls for stock data retrieval.
   - `summary.py` - Generates summaries using the API calls.
   - `fetch_calls.py` - Main class for communicating the frontend and the backend

## Starting the System
**Frontend/Backend**:
- Open the terminal and navigate to the `Frontend` directory.
- Run `npm install` to install dependencies.
- Start the server with:
  - `npm run dev`

## Stopping the System
- **Terminal**: Close the terminal session running the server to stop it.
- **VSCode**: Click the trash can icon in the Terminal panel to terminate the process or by pressing `Ctrl+C` (or `Cmd+C` on Mac) in the terminal window where the server is running.

## Troubleshooting
- If the server fails to start due to a port conflict, ensure no other services are using the same port (i.e. port 5173 for the frontend).
- If you encounter any errors related to missing modules, you can rerun `npm install` to make sure that all dependencies are installed.
## Source of Errors
- Open the Developer Tools in your browser using `F12` or `Ctrl+Shift+I` and check the Console tab for any frontend errors
- Usually any errors on the backend will be displayed in the terminal.
