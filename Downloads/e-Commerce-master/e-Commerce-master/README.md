
# Shoply

Welcome to **Shoply**, an advanced Angular-based ecommerce application designed to provide a seamless shopping experience. This platform enables users to explore a wide range of products with powerful filtering, sorting, and viewing options. Whether you're searching for specific items or browsing through categories, Shoply ensures a user-friendly and efficient shopping journey.

## Key Features

- **Product Catalog**: Browse an extensive range of products, categorized for easy navigation.
- **Product Details**: Access comprehensive information about each product, including images, descriptions, and prices.
- **Sorting and Pagination**: Organize products by price, popularity, and other criteria, with convenient pagination controls.
- **Suggested Products**: Discover related products tailored to your preferences.
- **Advanced Filtering**: Narrow down your search by category, price range, and other attributes.
- **Search Functionality**: Quickly find products using a robust search feature. 🔍
- **Dynamic Views**: Switch between list and grid views to suit your browsing preferences.
- **Price Range Slider**: Adjust your budget with a responsive price range slider.
- **Shopping Cart & Checkout**: Manage your cart, review your order, and proceed to payment with ease. 🛒
- **Local Storage Integration**: Save wishlist items and cart contents in local storage, ensuring that your selections persist even after refreshing the page.
- **End-to-End Testing**: Ensure quality and reliability with comprehensive tests using Cypress.

## Tech Stack

- **Client:** Angular, PrimeNG, PrimeFlex, Apollo Client
- **Server:** GraphQL
- **Tests:** Cypress

## Running End-to-End Tests

To execute the end-to-end tests, navigate to the project root directory and run:

```bash
npx cypress open
```

## Running the Application Locally

1. **Clone the Repository**

   ```bash
   git clone https://github.com/golubovicluka/ecommerce.git
   ```

2. **Navigate to the Project Directory**

   ```bash
   cd ecommerce
   ```

3. **Install Dependencies**

   ```bash
   npm install
   ```

4. **Start the Angular Development Server**

   ```bash
   ng serve
   ```

   The application will be available at `http://localhost:4200`.


5. **GraphQL Server**
   Install Apollo and GraphQL packages
This adds support for GraphQL and Apollo Client in your Angular project.

````npm install apollo-angular @apollo/client graphql
Create a GraphQL module for Apollo configuration
Set up a new file to connect Apollo Client to the EscuelaJS GraphQL API.

Create a file: src/app/graphql.module.ts

Use the API endpoint: https://api.escuelajs.co/graphql

Import GraphQLModule in your AppModule
This makes the GraphQL client available throughout the app.

Also import HttpClientModule (required by Apollo)

Create services to send GraphQL queries/mutations
Use Apollo's watchQuery for fetching data and mutate for actions like user registration.

Example services:

ProductsService → to get products, categories, etc.

Use those services in your components
Inject the service in your component and call the appropriate method to interact with the API.

 API Endpoint Used

````https://api.escuelajs.co/graphql
You can explore this API directly using a GraphQL playground or your browser.

