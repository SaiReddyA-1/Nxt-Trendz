# Nxt Trendz - Cart Features

In this project, let's build **Nxt Trendz - Cart Features** by applying the concepts we have learned so far.

### Refer to the video below:

<br/>
<div style="text-align: center;">
  <a href="https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-output.mp4" target="_blank" rel="noopener noreferrer">
    <video style="max-width:70%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12);outline:none;" loop="true" autoplay="autoplay" controls="controls" muted>
      <source src="https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-output.mp4" type="video/mp4">
    </video>
  </a>
</div>
<br/>

### Design Files

- [Extra Small (Size < 576px) and Small (Size >= 576px)](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-sm-output-v0.png)
- [Medium (Size >= 768px), Large (Size >= 992px) and Extra Large (Size >= 1200px)](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-lg-output.png)

### Set Up Instructions

- Download dependencies by running `npm install`
- Start up the app using `npm start`

### Completion Instructions

#### Functionality to be added

The app must have the following functionalities:

- When an unauthenticated user tries to access the **Cart** Route, the page should redirect to the **Login** Route.

- **Feature 1:**

  - When an authenticated user tries to add the same product multiple times:
    - The quantity of the product should update accordingly, and the count of cart items in the header should remain the same.

- **Feature 2:**

  - Display the total amount and number of items in the cart on the **Cart** Route.

- **Feature 3:**

  - In each cart item:
    - Clicking the plus icon should increment the product quantity by one.
    - Clicking the minus icon should decrement the product quantity by one.
    - If the quantity of a product is one and the minus icon is clicked, the respective product should be removed from the cart.
    - Based on the product quantity, update the product price and the Cart Summary, i.e., the total cost.

- **Feature 4:**

  - When an authenticated user clicks the remove button, the cart item should be removed from the cart list.

- **Feature 5:**

  - When an authenticated user clicks the **Remove All** button, remove all cart items from the cart and display the [Empty Cart View](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-empty-cart-view.png).

- The `CartContext` object has the following properties:
  - `cartList`: Stores the cart items.
  - `removeAllCartItems`: Removes all cart items from `cartList`.
  - `addCartItem`: Adds a cart item to `cartList`.
  - `removeCartItem`: Removes a cart item from `cartList`.
  - `incrementCartItemQuantity`: Increases the quantity of a product in `cartList`.
  - `decrementCartItemQuantity`: Decreases the quantity of a product in `cartList`.

#### Components Structure

<div style="text-align: center;">
  <img src="https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-component-structure-breakdown.png" alt="component structure breakdown" style="max-width:100%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12)">
</div>

#### Implementation Files

Use these files to complete the implementation:

- `src/App.js`
- `src/components/Cart/index.js`
- `src/components/Cart/index.css`
- `src/components/CartItem/index.js`
- `src/components/CartItem/index.css`
- `src/components/CartSummary/index.js`
- `src/components/CartSummary/index.css`

### Quick Tips

- The `line-height` CSS property sets the height of a line box. It's commonly used to set the distance between lines of text.

  ```css
  line-height: 1.5;


  ![line height](https://assets.ccbp.in/frontend/react-js/line-height-img.png)

- The array method `find()` returns the first item's value that satisfies the provided testing function. If no item is found, it returns `undefined`.

  **Syntax**: `arr.find(Testing Function)`

### Important Note

**The following instructions are required for the tests to pass:**

- Use `BsPlusSquare` and `BsDashSquare` icons from `react-icons` for the **plus** and **minus** buttons in the cart item.
- Each cart item should include two HTML button elements with `data-testid` attributes set to **plus** and **minus**, respectively.
- Use `AiFillCloseCircle` icon from `react-icons` for the **remove** button in each cart item.
- Each cart item should include an HTML button element with a `data-testid` attribute set to **remove**.
- Ensure the product image in the **Cart Item** Route has an `alt` attribute set to the product title.

### Resources

#### Colors

- Hex: #0b69ff
- Hex: #171f46
- Hex: #616e7c
- Hex: #ffffff

#### Font-families

- Roboto
