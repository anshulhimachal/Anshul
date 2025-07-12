
# Shoply

Welcome to **Shoply**, an advanced Angular-based ecommerce application designed to provide a seamless shopping experience. This platform enables users to explore a wide range of products with powerful filtering, sorting, and viewing options. Whether you're searching for specific items or browsing through categories, Shoply ensures a user-friendly and efficient shopping journey.

## Key Features

**Explore Products**: You can browse through a big collection of products, all neatly sorted into categories.

**See Details**: Click on any product to see its pictures, price, and description.

**Sort & Browse Easily**: Sort items by price or popularity, and move through pages easily.

**Get Suggestions**: We’ll show you similar or recommended products you might like.

**Smart Filters**: Want something within a budget or a specific category? Use filters to narrow it down.

**Search Anything**: Just type in what you’re looking for — our search bar finds it fast! 🔍

**Your View, Your Way**: Choose between list view or grid view, whichever you like more.

**Set a Budget**: Use a slider to set your price range — no typing needed!

**Easy Cart & Checkout**: Add items to your cart, check your order, and place it without any hassle. 🛒

**Saved Automatically**: Your cart and wishlist are saved in your browser — even if you refresh or come back later.

**Fully Tested**: The whole app is tested using Cypress, so everything works smoothly and reliably.

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

