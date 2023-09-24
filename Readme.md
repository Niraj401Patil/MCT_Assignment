## Beer project :

## Overview

This web application allows users to search for products effectively, reset the product list, and paginate through the product results. It displays products includes a search bar, reset button, and pagination controls.

## How it Works

- **Search Functionality:** Users can enter a search term in the input field and click the "Search" button. The JavaScript code filters the product list based on the user's search term, and the matching products are displayed. 

- **Reset Button:** Clicking the "Reset" button restores the original list of products fetched from the API.

- **Pagination:** Products are displayed in rows of 4 per row, and the app supports pagination. Users can click on the page numbers at the bottom to navigate through the product pages.

- **Fetching Data:** The app fetches product data from an external API (https://api.punkapi.com/v2/beers?page=1&per_page=60) using a `fetch` request. The data is retrieved in JSON format and stored in the `filteredProducts` variable.

- **Displaying Data:** JavaScript code dynamically creates HTML elements for each product, including an image and name, and displays them in rows and columns.

- **CSS Styling:** CSS styles are applied to create an attractive and user-friendly interface, including styling for the search container, product rows, product cards, images, and pagination.

## JavaScript Functionality

- **Fetching Data:** The `fetchProducts` function is responsible for fetching product data from the API using the `fetch` API. It retrieves the data and stores it in the `filteredProducts` array.

- **Displaying Data:** The `displayProducts` function is used to display products on a specific page. It calculates the start and end indices for the products to be displayed based on the current page and the specified number of products per page. It then creates HTML elements for each product, including an image and name, and appends them to the product container.

- **Pagination:** The `updatePaginationButtons` function generates the pagination buttons based on the number of pages required and updates the displayed products when a page number is clicked.

- **Search and Reset:** Event listeners are set up for the search and reset buttons. The search button filters the product list based on the user's search term and updates the display. The reset button restores the original list of products by refetching data from the API.

## Setup and Usage

1. Clone or download the repository.
2. Open `index.html` in your web browser to run the application.
3. Enter a search term in the input field and click "Search" to filter products.
4. Click "Reset" to restore the original product list.
5. Use the pagination buttons to navigate through the product pages.

The app provides a user-friendly interface for searching and browsing products with efficient pagination, making it easy for users to find the products they are looking for.
