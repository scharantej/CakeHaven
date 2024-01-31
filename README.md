## Design: Sweets Online Business Promotion Website

### HTML Files

1. **Home Page**: (`index.html`)
   - Visually appealing landing page introducing the online sweets business.
   - Displays high-quality images of the sweets and baked goods.
   - Includes a brief overview of the business and its products.
   - Features a clear call-to-action button for users to browse the products.

2. **Products Page**: (`products.html`)
   - Displays a comprehensive list of products offered by the business.
   - Each product entry includes an appealing image, product name, brief description, and price.
   - Provides a prominent button or link for users to add the product to their shopping cart.

3. **Cart Page**: (`cart.html`)
   - Displays the products currently in the user's shopping cart.
   - Includes the product name, quantity, price, and subtotal for each item.
   - Provides options for updating quantities, removing items, or proceeding to checkout.

4. **Checkout Page**: (`checkout.html`)
   - Facilitates the checkout process for users to complete their purchase.
   - Collects necessary details like shipping address, billing address, and payment information.
   - Offers different payment options and provides an intuitive checkout flow.

5. **Contact Page**: (`contact.html`)
   - Provides contact information for the business, including address, phone number, and email address.
   - Includes a contact form for users to send inquiries, feedback, or specific questions.

### Routes

1. **Home Route**: (`@app.route('/', methods=['GET'])`)
   - Renders the home page (`index.html`) when a user visits the website.

2. **Products Route**: (`@app.route('/products', methods=['GET'])`)
   - Renders the products page (`products.html`) showcasing the list of available sweets and baked goods.

3. **Cart Route**: (`@app.route('/cart', methods=['GET', 'POST'])`)
   - Handles adding products to the shopping cart and displays the current cart contents (`cart.html`).
   - Differentiates between GET requests for displaying the cart and POST requests for adding items.

4. **Checkout Route**: (`@app.route('/checkout', methods=['GET', 'POST'])`)
   - Renders the checkout page (`checkout.html`) and manages the checkout process.
   - Handles both GET requests for displaying the page and POST requests for processing checkout data.

5. **Contact Route**: (`@app.route('/contact', methods=['GET', 'POST'])`)
   - Renders the contact page (`contact.html`) and handles user inquiries.
   - Processes POST requests when users submit the contact form, sending their messages to the business.