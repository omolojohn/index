# *Testing Checklist for Shopping Cart Website*

## *1. Functional Testing*  
### *User Authentication*  
- [✅] Login with a valid token (Buyer, Seller, Admin).  
- [✅] Attempt login with an invalid token and verify error handling.  
- [✅] Verify session persistence (e.g., staying logged in after a page refresh).  
- [✅] Test logout functionality and ensure users are redirected appropriately.  

### *Product Management (Seller Role)*  
- [✅] Add a new product with all required details (name, price, description, image, category).  
- [✅] Attempt to add a product with missing details and verify validation messages.  
- [✅] Edit an existing product and ensure changes are saved.  
- [✅] Delete a product and confirm it no longer appears in listings.  

### *Cart Functionality (Buyer Role)*  
- [✅] Add items to the cart and verify they appear correctly.  
- [✅] Increase/decrease item quantity and ensure price updates accordingly.  
- [✅] Remove an item from the cart and confirm it's deleted.  
- [✅] Attempt checkout with an empty cart and check for errors.  

### *Checkout Process*  
- [✅] Proceed to checkout with valid items and verify the order summary.  
- [✅] Apply discount codes and ensure they update the total price correctly.  
- [✅] Complete payment using different payment methods and verify success/failure messages.  
- [✅] Confirm order details in the database after a successful purchase.  

### *Order Management*  
- [✅] Buyers should see their order history with correct details.  
- [✅] Sellers should receive notifications when an order is placed.  
- [✅] Admins should see all orders and be able to manage them.  

### *Admin Controls*  
- [✅] Verify admin login and dashboard access.  
- [✅] Test product moderation (approving/rejecting products).  
- [✅] Ensure the admin can manage users (ban/unban, change roles).  

---

## *2. UI/UX Testing*  
- [✅] Verify navigation across pages (Login, Product Listing, Cart, Checkout, Order History).  
- [✅] Test responsiveness on different devices (desktop, tablet, mobile).  
- [☑️] Check for broken links or missing images.  
- [✅] Ensure buttons, menus, and popups function as expected.  
- [✅] Validate proper error messages for incorrect user actions.  

---

## *3. Performance Testing*  
- [☑️] Measure page load speed for home, product, cart, and checkout pages.  
- [☑️] Simulate 100+ users browsing and adding items to the cart to test load handling.  
- [☑️] Analyze checkout performance under heavy traffic to identify bottlenecks.  
- [☑️] Monitor database queries to optimize response times.  

---

## *4. Security Testing*  
- [☑️] Test input fields for SQL Injection and XSS attacks.  
- [☑️] Ensure token-based authentication is secure (tokens shouldn’t be guessable).  
- [☑️] Check if login sessions expire correctly after logout.  
- [☑️] Verify access control (buyers shouldn’t access seller/admin features).  
- [☑️] Test payment security (sensitive data should be encrypted and not stored improperly).  

---

## *5. Integration Testing*  
- [☑️] Verify payment gateway integration with test transactions.  
- [☑️] Ensure order confirmation emails are sent successfully.  
- [☑️] Test integration with third-party APIs (e.g., shipping, analytics).  

---

## *6. Usability Testing*  
- [✅] Have real users test product search, checkout, and account management.  
- [✅] Gather feedback on ease of use and make UI improvements.  
- [✅] Fix any unclear error messages or confusing UI elements.  

---

## *7. Compatibility Testing*  
- [✅] Test across browsers (Chrome, Firefox, Safari, Edge).  
- [✅] Verify functionality on mobile devices (Android/iOS).  
- [✅] Ensure all interactive elements work on touchscreen devices.  

## Key
 .✅ - The ones I can do. <br>
 .☑️ -The ones I can do research on.
