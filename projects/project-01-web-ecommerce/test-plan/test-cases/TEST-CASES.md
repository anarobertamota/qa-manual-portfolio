# Test Cases — Project 01 (Web E-commerce Application)

## Document Information

- Project: Project 01 — Web Application Testing (E-commerce)
- Document Type: Test Cases
- Version: 1.0
- Author: Ana Roberta Mota
- Date: [Insert date]

---

## Legend

- Priority: High / Medium / Low
- Severity: Critical / High / Medium / Low
- Status: Not Executed / Pass / Fail / Blocked

---

# 1. User Registration

---

### TC-REG-001 — Register new user with valid data

- Priority: High  
- Preconditions: User is on Registration page  
- Steps:
  1. Enter valid name
  2. Enter valid email
  3. Enter valid password
  4. Confirm password
  5. Click "Register"
- Expected Result: User account is created and success message is displayed.

---

### TC-REG-002 — Register user with existing email

- Priority: High  
- Preconditions: Email is already registered  
- Steps:
  1. Enter name
  2. Enter an email already registered
  3. Enter password
  4. Confirm password
  5. Click "Register"
- Expected Result: System displays error message indicating email is already in use.

---

### TC-REG-003 — Register user with invalid email format

- Priority: Medium  
- Preconditions: User is on Registration page  
- Steps:
  1. Enter valid name
  2. Enter invalid email (example: ana@com)
  3. Enter valid password
  4. Confirm password
  5. Click "Register"
- Expected Result: System blocks submission and displays validation message for invalid email.

---

### TC-REG-004 — Register user with empty required fields

- Priority: High  
- Preconditions: User is on Registration page  
- Steps:
  1. Leave all required fields blank
  2. Click "Register"
- Expected Result: System highlights required fields and shows validation messages.

---

### TC-REG-005 — Register user with mismatched password confirmation

- Priority: High  
- Preconditions: User is on Registration page  
- Steps:
  1. Enter valid name
  2. Enter valid email
  3. Enter password
  4. Enter a different password in confirm password field
  5. Click "Register"
- Expected Result: System displays error message indicating passwords do not match.

---

# 2. Login / Logout

---

### TC-LOG-001 — Login with valid credentials

- Priority: High  
- Preconditions: Registered user exists  
- Steps:
  1. Navigate to Login page
  2. Enter valid email
  3. Enter valid password
  4. Click "Login"
- Expected Result: User is successfully logged in and redirected to the homepage/dashboard.

---

### TC-LOG-002 — Login with invalid password

- Priority: High  
- Preconditions: Registered user exists  
- Steps:
  1. Navigate to Login page
  2. Enter valid email
  3. Enter invalid password
  4. Click "Login"
- Expected Result: System displays error message and denies access.

---

### TC-LOG-003 — Login with unregistered email

- Priority: High  
- Preconditions: Email does not exist in system  
- Steps:
  1. Navigate to Login page
  2. Enter unregistered email
  3. Enter password
  4. Click "Login"
- Expected Result: System displays error message "User not found" or equivalent.

---

### TC-LOG-004 — Logout user successfully

- Priority: High  
- Preconditions: User is logged in  
- Steps:
  1. Click "Logout"
- Expected Result: User is logged out and redirected to login or home page.

---

# 3. Product Search and Filtering

---

### TC-SRC-001 — Search for an existing product

- Priority: High  
- Preconditions: Products exist in the catalog  
- Steps:
  1. Enter product name in search bar
  2. Click "Search"
- Expected Result: System displays products matching the search term.

---

### TC-SRC-002 — Search for a non-existing product

- Priority: Medium  
- Preconditions: Products exist in the catalog  
- Steps:
  1. Enter a random non-existing product name
  2. Click "Search"
- Expected Result: System displays "No results found" message.

---

### TC-FLT-001 — Apply product filter successfully

- Priority: Medium  
- Preconditions: Filter options are available  
- Steps:
  1. Open product listing page
  2. Apply a category filter
  3. Apply a price filter (if available)
- Expected Result: System updates results according to applied filters.

---

### TC-FLT-002 — Clear filters

- Priority: Medium  
- Preconditions: Filters applied  
- Steps:
  1. Click "Clear filters"
- Expected Result: All filters are removed and full product list is displayed.

---

# 4. Product Details Page

---

### TC-PDP-001 — Open product details page

- Priority: High  
- Preconditions: Products exist in catalog  
- Steps:
  1. Click on a product from listing page
- Expected Result: Product details page loads with correct product name, price, and description.

---

### TC-PDP-002 — Verify product image display

- Priority: Low  
- Preconditions: Product has an image  
- Steps:
  1. Open product details page
  2. Verify image loads properly
- Expected Result: Product image is displayed correctly without broken links.

---

# 5. Cart Management

---

### TC-CART-001 — Add product to cart from product details page

- Priority: High  
- Preconditions: Product exists and is available  
- Steps:
  1. Open product details page
  2. Click "Add to cart"
- Expected Result: Product is added to cart and cart icon updates quantity.

---

### TC-CART-002 — Add multiple products to cart

- Priority: High  
- Preconditions: Multiple products exist  
- Steps:
  1. Add Product A to cart
  2. Add Product B to cart
  3. Open cart page
- Expected Result: Cart displays both products correctly.

---

### TC-CART-003 — Update product quantity in cart

- Priority: High  
- Preconditions: Product is already in cart  
- Steps:
  1. Open cart page
  2. Increase quantity of product
  3. Click "Update" (if applicable)
- Expected Result: Quantity updates correctly and total price recalculates.

---

### TC-CART-004 — Remove product from cart

- Priority: High  
- Preconditions: Product is already in cart  
- Steps:
  1. Open cart page
  2. Click "Remove" on product item
- Expected Result: Product is removed and cart total updates.

---

### TC-CART-005 — Cart empty message

- Priority: Medium  
- Preconditions: Cart is empty  
- Steps:
  1. Open cart page
- Expected Result: System displays "Your cart is empty" message.

---

# 6. Checkout

---

### TC-CHK-001 — Proceed to checkout with products in cart

- Priority: High  
- Preconditions: User has products in cart  
- Steps:
  1. Open cart page
  2. Click "Proceed to checkout"
- Expected Result: System redirects to checkout page.

---

### TC-CHK-002 — Checkout with missing required shipping information

- Priority: High  
- Preconditions: User is on checkout page  
- Steps:
  1. Leave required shipping fields empty
  2. Click "Place order"
- Expected Result: System blocks submission and shows validation messages.

---

### TC-CHK-003 — Checkout with valid shipping information

- Priority: High  
- Preconditions: User is on checkout page with items in cart  
- Steps:
  1. Fill in all required shipping fields with valid data
  2. Click "Place order"
- Expected Result: Order is placed successfully and confirmation page is displayed.

---

# 7. Order Confirmation

---

### TC-ORD-001 — Validate order confirmation page details

- Priority: High  
- Preconditions: Order has been placed  
- Steps:
  1. Place a valid order
  2. Verify confirmation page
- Expected Result: System displays order number, summary, and success message.

---

### TC-ORD-002 — Validate cart is cleared after order placement

- Priority: Medium  
- Preconditions: Order placed successfully  
- Steps:
  1. Complete checkout
  2. Navigate to cart page
- Expected Result: Cart is empty after successful order.

---

# 8. Exploratory Testing Notes (Optional)

---

### TC-EXP-001 — Exploratory test session on cart and checkout flow

- Priority: Medium  
- Preconditions: User can browse products  
- Steps:
  1. Navigate between product listing and cart multiple times
  2. Add/remove products quickly
  3. Refresh page during checkout
  4. Attempt invalid inputs in shipping fields
- Expected Result: System remains stable and no unexpected errors occur.
