# Models and Relations

## Auth
- SupplierEmployees accounts (id, supplier_group(admin or manager) , name, email, password, created on, updated on)
- Users accounts (id, name, email, password, created on, updated on)

- Supplier-Account (id, supplierEmployee acount id, supplier id)

## Supplier Groups Authorization Management
- Supplier Groups (id, type(admin or manager), [API's allowed or not] <br/>
LOGIC : Accounts -> Supplier or Users -> IF Supplier-> Admin, Manager -> Managers can do everything except profile updates, and delete.

## Profile
- Supplier profile (1-1 with suppliers account, phone, geolocation, description, restrictions, created on, updated on)
- User profile (1-1 with users account, phone, created on, updated on)

## Subscription Handling
- Supplier-Users (id, supplier id, user id, created on) Many-Many relation between suppliers and users

## Deals/Items
- Items (item id, supplier id, name, type, item deal expiration date, stock available, description, restriction, created on, updated on) One store can have many items
- Wishlist (user id, tags, created on, updated on)
