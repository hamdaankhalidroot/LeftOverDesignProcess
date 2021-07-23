# Models and Relations

## Auth

- SupplierEmployees accounts (id, supplierStore id, supplier_group(admin or manager) , name, email, password, created on, updated on)

- Users accounts (id, name, email, password, created on, updated on)


## Supplier Emplyoyee Store Management

- SupplierStore-SupplierEmployeees (id, SupplierEmployeees id, SupplierStore id)


## Profile

- supplierStore profile (supplierStore id, name, email, phone, geolocation, description, restrictions, created on, updated on)

- User profile (1-1 with users account, phone, created on, updated on)


## Subscription Handling

- Supplier-Users (id, supplierStore id, user id, created on) Many-Many relation between supplierStores and users


## Deals/Items

- Items (item id, supplierStore id, name, type, item deal expiration date, stock available, description, restriction, created on, updated on) One store can have many items

- Wishlist (user id, tags, created on, updated on)
