# E-Commerce App

## Overview

This is an E-Commerce web application built with **React**, **Redux Toolkit**, and **Firebase**. The application features global state management, Firebase authentication, product filtering, cart management, and order tracking.

---

## Features

* **User Authentication:** Signup, Login with form validation and Firebase Authentication.
* **Global State Management:** Implemented using Redux Toolkit with slices for `auth`, `products`, and `cart`.
* **Asynchronous Thunks:** Handling Login, Signup, Add/Remove from cart, and product fetching.
* **Product Filtering & Search:** Sidebar to filter products by price and categories; search products by name.
* **Cart Functionality:** Add to cart, increment/decrement quantity, remove products, total price calculation.
* **Orders Page:** View summary of all placed orders.
* **Routing:** Includes `/signup`, `/signin`, `/cart`, `/myorders`, and a fallback 404 page.

---

## Project Structure

```
/src
|-- components
|-- pages
|-- redux
|   |-- store.js
|   |-- slices
|       |-- authSlice.js
|       |-- productSlice.js
|       |-- cartSlice.js
|-- App.js
|-- index.js
```

---

## Available Routes

* `/` : Homepage with products, filters, and search.
* `/signup` : User registration.
* `/signin` : User login.
* `/cart` : View and manage cart items.
* `/myorders` : View past orders.
* `*` : Fallback route displaying "Page Not Found".

---

## Installation

1. **Clone the repository:**

```bash
git clone https://github.com/your-username/E-Commerce_App.git
cd E-Commerce_App
```

2. **Install dependencies:**

```bash
npm install
```

3. **Setup Firebase:**

* Create a Firebase project.
* Replace Firebase config in the app with your project credentials.

4. **Start the application:**

```bash
npm start
```

App will run on `http://localhost:3000/`.

---

## State Management (Redux Slices)

### Auth Slice

* Handles user authentication state.
* Async thunks: `loginUser`, `signupUser`.

### Product Slice

* Stores product list.
* Handles filters and search.

### Cart Slice

* Manage cart items, quantities, and total.
* Async thunks: `addToCart`, `removeFromCart`.

---

## Testing Criteria

* Home Page: Navbar conditionally displays Signin and Home before login.
* Signup & Signin: Validation with error messages via Toastify.
* Product Filters: Sidebar filters based on price and categories.
* Search: Search bar to filter products by name.
* Cart Management: Add to cart, quantity control, and removal.
* Orders: Summary of purchases or "No Orders Found" message.

---

## Contributing

Contributions are welcome! Please fork the repository, create a feature branch, and submit a pull request.

## Contact

For any queries or feedback, please contact:
**[n.pranideepreddy1999@gmail.com](mailto:n.pranideepreddy1999@gmail.com)**
