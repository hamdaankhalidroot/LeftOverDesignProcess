# Scenes and Functionalities

## Logic Encapsulation From Display

- A javascript application that models all functions and objects that are usually nested in components in React, in pure javascript. Then using this base library to render information on Web and App.

## Users

### Un-Authenticated Scenes
- Users Landing Page ( A landing page more targetted for Users )
  * An about section
  * Users value proposition
  * links to signup, login, blogs, contact us 
  
- Signup Page
  * Form to signup as a Store (Creates StoresProfile Admin and Store's Profile)
  * A way to switch to login
  * A way to navigate back to homescreen
  
- Login Page
  * Form to login
  * A way to switch to signup
  * A way to navigate back to landing page

### Authenticated Scenes
- Home Page
  * Link to logout
  * Link to edit profile page
  * Link to Subscriptions page
  * Link to Wishlist page
  * Locate & Subscribe to suppliers

- Edit Profile Page

- Subscriptions Page (edit, delete, add, subscribe to suppliers)

- Wishlist Page (CRUD wishes, view a list of wishes available in all published items)
  
## Suppliers

### Un-Authenticated Scenes
- Suppliers Landing Page ( A landing page more targetted for suppliers (grocery stores and food banks) )
  * An about section
  * Suppliers value proposition
  * links to signup, login, blogs, contact us
  
- Signup Page
  * Form to signup as Store (Can signup as an admin/ create a supplierStore!)
  * Form to signup as Employee of existing Store (Choose which store, await admin to approve)
  * A way to switch to login
  * A way to navigate back to homescreen 
  
- Login Page
  * Form to login
  * A way to switch to signup
  * A way to navigate back to landing page

### Authenticated Scenes
- Home Page
  * Link to logout
  * Link to edit profile page
  * Link to history page
  * Link to subscribed users dashboard page
  * create deals
 
- Edit Profile Page (StoresProfile Admin only)

- History Page (View all past items published, re-publish them with slight edits)

- Subscribed Users Dashboard Page (View stats and info about users subscribed to the supplier)

