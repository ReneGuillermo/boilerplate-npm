# FreeCodeCamp NPM Package Management Project

## Overview
This is a FreeCodeCamp boilerplate project for learning Node.js and npm package management. It's a simple Express.js web application that serves static content and provides an API endpoint to display package.json information.

## Recent Changes
- **2024-09-25**: Initial Replit environment setup
  - Installed project dependencies with npm install
  - Updated server.js to bind to 0.0.0.0:5000 for Replit compatibility
  - Modified CORS settings to work with Replit's proxy environment
  - Configured workflow to run the Express server on port 5000
  - Set up deployment configuration for autoscale deployment

## Project Architecture
- **Backend**: Node.js with Express.js framework
- **Frontend**: Static HTML served by Express
- **Port**: 5000 (required for Replit environment)
- **Host**: 0.0.0.0 (required for Replit proxy)
- **API Endpoints**:
  - `/` - Serves the main HTML page
  - `/_api/package.json` - Returns package.json content as text
  - `/public/*` - Serves static assets (CSS, etc.)

## Key Files
- `server.js` - Main Express server application
- `package.json` - Project dependencies and scripts
- `views/index.html` - Main HTML page
- `public/style.css` - Styling for the application

## Development
- Uses `npm start` to run the server
- Server automatically restarts on changes in Replit environment
- CORS configured to work with FreeCodeCamp and Replit domains

## Deployment
- Configured for autoscale deployment on Replit
- Production uses the same `npm start` command
- No build step required (static files served directly)