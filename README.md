# Phone Search Webpage

This project is a responsive Phone Search webpage that allows users to search for phones from an external API and view detailed information about each phone. The project is styled using DaisyUI and Tailwind CSS with a custom "dracula" theme, and includes smooth animations and transitions for an enhanced user experience.

## Hosted Link

Check out the live site here: [Phone Search Live](https://navnitsingh0110.github.io/Phone-Search/)

## Project Overview

The webpage consists of the following key sections:

- **Navigation Bar:**  
  A header with the website title ("Hot Gadgets") and a "Sign Up" button.

- **Hero Header:**  
  A visually appealing banner featuring the product (e.g., "Apple iPhone 13 Pro Max") with a "Buy Now" button, accompanied by a brief description.

- **Search Section:**  
  A search input field where users can type keywords (e.g., "iphone", "samsung") to search for phones. The search functionality fetches data from an external API and displays a list of phone cards.

- **Phone Cards:**  
  Each phone is displayed as a card with its image, name, and a "Show Details" button. Clicking this button opens a modal with more information about the selected phone.

- **Modal:**  
  A popup that provides detailed information about the phone, including the image, brand, key features, and release date.

- **Footer:**  
  Contains company information and social media icons with hover effects.

## How I Accomplished the Task

### HTML & CSS

- **HTML Structure:**  
  The webpage is divided into semantic sections (`<nav>`, `<header>`, `<main>`, `<footer>`) for better organization and accessibility.

- **Styling:**  
  - **DaisyUI & Tailwind CSS:**  
    Utilized DaisyUI’s built-in themes (set to `dracula` via the `data-theme` attribute on the `<html>` tag) and Tailwind CSS utility classes for responsive design, layout, and styling.
  - **Custom Animations:**  
    Added a custom CSS keyframe animation (`fadeIn`) and hover transitions to elements like cards, buttons, and images. This creates smooth visual effects as elements load and when users interact with them.

### JavaScript Functionality

- **Fetching and Displaying Data:**
  - **`loadPhone(searchText, isShowAll)`:**  
    An asynchronous function that fetches phone data from an API based on the user’s search query.
  - **`displayPhones(phones, isShowAll)`:**  
    Renders the fetched phone data as individual cards. It also handles the "Show All" button, which displays more results if available.
  - **`searchHandler(isShowAll)`:**  
    Captures the search term from the input field, triggers the loading spinner, and calls `loadPhone` to fetch and display data.

- **Loading State:**
  - **`loading(isLoading)`:**  
    Toggles a loading spinner to provide visual feedback during data fetch operations.

- **Modal and Detailed View:**
  - **`showDetailsHandler(id)`:**  
    Fetches detailed information about a selected phone when the "Show Details" button is clicked.
  - **`showPhoneDetails(details)`:**  
    Populates and displays a modal with the phone’s image, name, brand, main features, and release date.

- **Interactivity Enhancements:**
  - Used **async/await** for cleaner asynchronous operations during API calls.
  - Added hover effects using Tailwind CSS transitions and custom CSS classes to improve the overall user interaction.

## Conclusion

This project integrates modern front-end tools and techniques to build a dynamic and responsive web application. The use of DaisyUI with Tailwind CSS for styling, combined with JavaScript for dynamic data handling, results in a user-friendly interface with engaging animations and transitions. The project is hosted on GitHub Pages and can be viewed via the provided link.

Happy Coding!
