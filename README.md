# **RR Music Library**

A web-based music library application that allows users to search and explore music tracks from the iTunes API. Built with React, the application provides an interactive interface to display search results with both simple and detailed views.

## Demo

Explore the live demo of the RR Music Library at https://tourmaline-speculoos-57772d.netlify.app/

## Technologies Used

- **Frontend:** React
- **Backend:** None (Uses iTunes API for data)
- **Version Control:** Git
- **Styles:** CSS (app.css, index.css)
- **Testing:** React Testing Library
- **Additional Libraries:** 
  - `@testing-library/jest-dom`: ^5.12.0
  - `@testing-library/react`: ^11.2.6
  - `@testing-library/user-event`: ^12.8.3
  - `react`: ^18.2.0
  - `react-dom`: ^18.2.0
  - `react-scripts`: ^5.0.1
  - `web-vitals`: ^1.1.1

## File Structure

- **src/**
  - **components/**
    - `Gallery.js`: Renders a list of `GalleryItem` components based on search results.
    - `GalleryItem.js`: Displays individual music items with toggleable views for simple and detailed information.
    - `SearchBar.js`: Provides a search form to filter music tracks.
  - `App.css`: Styles for the main application layout.
  - `App.js`: Main application component that manages state and handles search functionality.
  - `App.test.js`: Contains tests for the `App` component.
  - `index.css`: Global styles for the application.
  - `index.js`: Entry point of the React application.
  - `reportWebVitals.js`: Used for measuring performance metrics of the app.

- **public/**
  - `index.html`: HTML template for the application. Includes meta tags and links for icons.
  - `manifest.json`: Metadata for the web app including icons and theme colors.

## Installation

To install and run the project locally:

1. Clone the repository from [https://github.com/Shivnia/RR-Music-Library](https://github.com/Shivnia/RR-Music-Library) and navigate to the project directory.
2. Install the dependencies using npm: `npm install`.
3. Start the development server: `npm start`.
4. Open your browser and go to [http://localhost:3000/](http://localhost:3000/) to view the application.

## Technical Information

- **Frontend:** React with functional components and hooks (useState, useEffect).
- **API Integration:** Fetches data from the iTunes API based on user search terms.
- **Styling:** CSS modules for component-specific styles and global styling.


### Scripts

- `npm start`: Starts the development server.
- `npm build`: Creates a production build of the application.
- `npm test`: Runs tests for the application.
- `npm eject`: Exposes configuration files for customization.

### Browser Compatibility

- **Production:** Supports browsers with greater than 0.2% market share, excluding obsolete ones.
- **Development:** Supports the latest versions of Chrome, Firefox, and Safari.

## Contributing

To contribute to this project:

1. Fork the repository from https://github.com/Shivnia/RR-Music-Library
2. Create a new branch for your feature or fix.
3. Make your changes and commit them.
4. Push your changes to the new branch.
5. Open a pull request to the original repository.



## Issues

- **Known Issues:**
  - None 

- **Feature Requests:**
  - None
## Changelog

For detailed information about changes and version releases, see [CHANGELOG.md](#) (No Changelog as this is a solution branch for building a readme)

## API Documentation

The application interacts with the iTunes API. For details on the API endpoints used:

- **Reference Documentation:** Fetches data from `https://itunes.apple.com/search?term={searchTerm}`. The API returns search results with fields like `trackName`, `collectionName`, `artworkUrl100`, etc.
- **Tutorial Documentation:** To search for music, enter a term in the search bar. The application fetches and displays results based on the search term.
- **Conceptual Documentation:** The app sends search queries to the iTunes API and processes the response to display music tracks. The `Gallery` component renders a list of `GalleryItem` components, which provide detailed or simple views of the tracks.


