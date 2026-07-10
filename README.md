# Housing Listings Angular App

This project is an Angular application for browsing housing listings, filtering them by city, and viewing detailed information for each property. The app uses a mock API to load listing data and a reactive form for submitting an application.

## Features

- Browse a list of housing locations on the home page
- Filter listings by city with a search input
- Open a detail page for each location
- Submit a rental application form from the details page
- Uses Angular routing and standalone components

## Tech Stack

- Angular
- TypeScript
- CSS
- JSON Server for mock data

## Prerequisites

Make sure you have the following installed:

- Node.js
- npm

## Installation

1. Clone the repository
2. Install frontend dependencies:

```bash
npm install
```

3. Start the mock API server:

```bash
json-server --watch db.json --port 3000
```

> The app expects the mock API to be available at http://localhost:3000/locations.

## Run the application

Start the Angular development server:

```bash
npm start
```

Then open your browser at:

```text
http://localhost:4200/
```

## Available Scripts

```bash
npm start      # start the Angular dev server
npm run build  # build the app for production
npm run watch  # build in watch mode for development
```

## Project Structure

```text
src/
  app/
    home/           # Home page and listing filter
    details/        # Listing detail view and application form
    housing-location/  # Reusable listing card component
    housing.service.ts # API service for fetching housing data
    housinglocation.ts # Shared housing model
    routes.ts       # Angular route configuration
```

## Data Source

The application uses the mock database file [db.json](db.json), which contains sample housing locations. The data is served by JSON Server during local development.

## Notes

- The application form submission currently logs the submitted values to the browser console.
- The detail route is available at /details/:id.

## License

This project is open source and available under the MIT License.
