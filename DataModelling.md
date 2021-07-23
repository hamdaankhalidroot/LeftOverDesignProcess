# Models and Relations


## Auth

- supplierStore account (Admin Account) :=> (supplierStore id, name, email, password, created on, updated on)

- SupplierEmployee accounts (Manager Account) :=> (SupplierEmployee id, supplierStore id, adminApproved?, name, email, password, created on, updated on)

- Users accounts :=> (id, name, email, password, created on, updated on)


## Profile

- supplierStore profile :=> (supplierStore id, name, email, phone, geolocation, description, restrictions, created on, updated on)

- User profile :=> (1-1 with users account, phone, created on, updated on)


## Subscription Handling

- SupplierStore-Users :=> (id, supplierStore id, user id, created on) Many-Many relation between supplierStores and users


## Deals/Items

- Items :=> (item id, supplierStore id, name, type, item deal expiration date, stock available, description, restriction, created on, updated on) One store can have many items

- Wishlist :=> (user id, tags, created on, updated on)
