# React Products catalog
An online store for gadgets and accessories. It lets customers browse products, see information about them, choose different models, search and sort products, and add them to cart or favorites.
The application is implemented using React functional components and React Hooks. App navigation is implemented with React Router. Products and their details are fetched from the server.

Implemented according to the [Figma design](https://www.figma.com/file/T5ttF21UnT6RRmCQQaZc6L/Phone-catalog-(V2)-Original?type=design&node-id=0-1&mode=design).

# [DEMO](https://oksana-vas.github.io/product_catalog/)

## Technologies used
- React.js (JSX, React Router, React Context)
- Typescript
- Javascript
- CSS
- Sass (SCSS)
- Fetch, API
- BEM methodology

## Structure
- [Home page](#home-page)
- [Category page](#category-page)
- [Product details page](#product-details-page)
- [Cart page](#cart-page)
- [Favorites page](#favorites-page)
- [Search](#search)

### Home page
- A welcome slider that automatically slides every 5 seconds and lets users slide the pictures by pressing the arrow buttons or swiping pictures on mobile devices.
- Products slider with the ability to scroll products by pressing the arrow buttons or just swiping.

### Category page
- Users can sort products by age, name and price. All sorting parameters are saved in the URL.
- Implemented pagination with the ability to choose the number of products displayed on the page. In the case of numerous products and pages, pagination with dots is created.
- Search field with the ability for users to filter of find products by name. To avoid server overload, the debounce function is employed.

### Product details page
- The application loads product details from the server.
- Users have the option to select a color and capacity for the product. Photos of the product can be changed by either clicking on the thumbnails or swiping them on mobile devices.
- Users can add the product to their cart or mark it as a favorite.

### Cart page
- Users have the ability to change the quantity of products within the cart and remove items from it.
- The count of cart items is displayed near the Cart icon in the header.
- The total amount and quantity are automatically counted.
- Cart items are stored in the local storage.

### Favorites page
- Users can also add products to their favorites and remove them from there by clicking the heart button.
- The count of favorite items is displayed near the Favorites icon in the header.
- Favorite items are also stored in the local storage.

### Search
- Users can filter or find products in Category pages and Favorites page.
- Search field is implemented and adapted for all screen sizes and devices.
- Search also works with pagination and sorting.
- To avoid server overload, the debounce function is employed.
- The search parameters are also saved in the URL.
