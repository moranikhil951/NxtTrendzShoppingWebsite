# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)


In this project, let's build a **Nxt Trendz - Cart Features** 

### Refer to the video below:

<br/>
<div style="text-align: center;">
  <video style="max-width:70%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12);outline:none;" loop="true" autoplay="autoplay" controls="controls" muted>
    <source src="https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-output.mp4" type="video/mp4">
  </video>
</div>
<br/>

### Design Files

<details>
<summary>Click to view</summary>

- [Extra Small (Size < 576px) and Small (Size >= 576px)](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-sm-output-v0.png)
- [Medium (Size >= 768px), Large (Size >= 992px) and Extra Large (Size >= 1200px)](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-lg-output.png)

</details>

### Set Up Instructions

<details>
<summary>Click to view</summary>

- Download dependencies by running `npm install`
- Start up the app using `npm start`
</details>

### Completion Instructions

1. 
Exclusive Prime deals are for Prime Users.
All Products are for both Prime and Non-Prime users.


2. API Call Possible Views
2.1 Success View
When the Prime User is logged in and accessed Prime Deals Section then we should show the Exclusive Prime Deals section.

2.2 Failure View
When the Non-prime User is logged in and accessed Prime Deals Section then we should show the Get Exclusive Deals section.

Reasons for API Call Failure :
Sending UnAuthorized User credentials
Not specifying Authorization header
Using the wrong HTTP method
2.3Loading View
When the Prime or Non-prime User is logged in and accessed Prime Deals Section, we should show the Loading view until data is in progress.


3. 
3.1 File: src/components/AllProductsSection/index.js
    File: src/components/Cart/index.js
    File: src/components/Header/index.js
    File: src/components/Home/index.js
    File: src/components/LoginForm/index.js
    File: src/components/NotFound/index.js
    File: src/components/PrimeDealsSection/index.js
    File: src/components/ProductCard/index.js
    File: src/components/Products/index.js
    File: src/components/ProductItemDetails/index.js
    File: src/components/CartItem/index.js
    File: src/components/CartListView/index.js
    File: src/components/CartSummary/index.js
    File: src/components/EmptyCartView/index.js
    File: src/components/FilterGroup/index.js
    File: src/components/similarProductItem/index.js
    File: src/components/ProductsHeader/index.js
    File: src/components/ProtectedRoute/index.js



4. 

4.1 State Variable-isLoading
isLoading is used to handle Success View, Loading View only. 

4.2 State Variable-apiStatus
apiStatus is used to handle Success, Failure and Loading Views.


5. React Icons
react-icons is a third-party package contains bundle of icons like bootstrap, font awesome, material icons etc..,
 
 ####to install react icons - npm install react-icons###

 Importing React Icons
The First letters of the icon indicates the category of the Icon.

Each category of Icons have import statements separately, go to the category and copy the import statement.

6. React Context
Context is a mechanism that provides different Components and allows us to pass data without doing prop drilling.

6.1 Creating Context
      ===React.createContext(INITIAL_VALUE)===

6.2 Context Properties
    The Context object provides two properties.

     6.2.1  Consumer
     6.2.2  Provider

 6.3 How to Access the Value?
We can access the value in the Context using Consumer Component provided by the Context Object.

6.4 Consumer Component
Syntax: <ContextObject.Consumer>
  {/*callback function*/}
</ContextObject.Consumer>

6.5 Provider
Provider Component updates the value of Context.
When the provider updates context, all the nested consumers of that provider will be re-rendered.
Updated context value can only be accessed by the consumers nested within the provider.
syntax : <ContextObject.Provider value={/* some value */}>
   ...
<ContextObject.Provider/>






<details>
<summary>Functionality to be added</summary>
<br/>

The app must have the following functionalities

- When an unauthenticated user tries to access the **Cart** Route, then the page should be navigated to **Login** Route

- Following are the features to be implemented

  - Feature 1

    - When an authenticated user tries to add the same product multiple times
      - The quantity of the product should be updated accordingly, and the count of the cart items in the header should be remained same

  - Feature 2

    - The total amount and number of items in the cart should be displayed in the **Cart** Route

  - Feature 3

    - In each cart item in the cart
      - When the plus icon is clicked, then the quantity of the product should be incremented by one
      - When the minus icon is clicked, then the quantity of the product should be decremented by one
      - When the quantity of the product is one and the minus icon is clicked, then the respective product should be removed from the cart
      - Based on the quantity of the product, the product price and the Cart Summary, i.e the total cost should be updated accordingly

  - Feature 4

    - When an authenticated user clicks on the remove button, cart item should be removed from the cart list

  - Feature 5

    - When an authenticated user clicks on the **Remove All** button, all the cart items should be removed from the cart and [Empty Cart View](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-empty-cart-view.png) should be displayed

- The `CartContext` has an object as a value with the following properties
  - `cartList` - this key stores the cart items
  - `removeAllCartItems` - this method is used to remove all the cart items in the `cartList`
  - `addCartItem` - this method adds the cart item to the `cartList`
  - `removeCartItem` - this method removes the cart item from the `cartList`
  - `incrementCartItemQuantity` - this method increases the quantity of a product in the `cartList`
  - `decrementCartItemQuantity` - this method decreases the quantity of a product in the `cartList`

</details>

<details>
<summary>Components Structure</summary>

<br/>
<div style="text-align: center;">
    <img src="https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-component-structure-breakdown.png" alt="component structure breakdown" style="max-width:100%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12)">
</div>
<br/>

</details>

<details>
<summary>Implementation Files</summary>
<br/>

Use these files to complete the implementation:

- `src/App.js`
- `src/components/Cart/index.js`
- `src/components/Cart/index.css`
- `src/components/CartItem/index.js`
- `src/components/CartItem/index.css`
- `src/components/CartSummary/index.js`
- `src/components/CartSummary/index.css`
</details>

### Quick Tips

<details>
<summary>Click to view</summary>
<br>

- The `line-height` CSS property sets the height of a line box. It's commonly used to set the distance between lines of text

  ```
  line-height: 1.5;
  ```

    <br/>
    <img src="https://assets.ccbp.in/frontend/react-js/line-height-img.png" alt="line height" style="width:90%; max-width: 600px;"/>

- The array method `find()` returns the first item's value that satisfies the provided testing function. If no item is found, it returns `undefined`

  **Syntax**: `arr.find(Testing Function)`

</details>

### Important Note

<details>
<summary>Click to view</summary>

<br/>

**The following instructions are required for the tests to pass**

- `BsPlusSquare`, `BsDashSquare` icons from `react-icons` should be used for **plus** and **minus** buttons in cart item
- The Cart Item should consist of two HTML button elements with data-testid attribute values as **plus** and **minus** respectively
- `AiFillCloseCircle` icon from react-icons should be used for **remove** button in cartItem
- The Cart Item should consist of an HTML button element with data-testid attribute values as **remove**
- The product image in **Cart Item** Route should have the alt as `title` of the product

- Prime User credentials

  ```text
   username: rahul
   password: rahul@2021
  ```

- Non-Prime User credentials

  ```text
   Username: henry
password: henry_the_developer
  ```

</details>

### Resources

<details>
<summary>Colors</summary>

<br/>

<div style="background-color: #0b69ff; width: 150px; padding: 10px; color: white">Hex: #0b69ff</div>
<div style="background-color: #171f46; width: 150px; padding: 10px; color: white">Hex: #171f46</div>
<div style="background-color: #616e7c; width: 150px; padding: 10px; color: white">Hex: #616e7c</div>
<div style="background-color: #ffffff; width: 150px; padding: 10px; color: black">Hex: #ffffff</div>

</details>

<details>
<summary>Font-families</summary>

- Roboto


==>  Overview  <==
This is the frontend of a fully responsive e-commerce website built with modern web technologies. The project focuses on providing a seamless user experience for browsing and purchasing products. It includes features like product listings, shopping cart, and a user-friendly interface.

==>  Features  <==
Product Display: Browse through a variety of products with detailed information such as images, prices, and descriptions.
Search Functionality: Users can search for products by name or category.
Shopping Cart: Add items to the cart, view the total price, and adjust quantities.
Responsive Design: The site is optimized for various screen sizes, providing a smooth experience on both mobile and desktop devices.

 ==> Technologies Used <==
HTML5: For structuring the web pages.
CSS3: For styling, including Flex box and CSS Grid for layout.
JavaScript (ES6+): For dynamic interactions and logic.
React.js: A JavaScript library for building the user interface.
React Router: For handling page navigation.
Axios or Fetch API: For HTTP requests to any backend API.
Bootstrap or Tailwind CSS: For responsive and modern design (if used).