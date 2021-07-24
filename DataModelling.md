# Models and Relations

- https://simpleisbetterthancomplex.com/tutorial/2018/01/18/how-to-implement-multiple-user-types-with-django.html

## Auth
- Accounts (Extend AbstractUser) :=> Add fields => is_supplier_store || is_user || is_supplier_employee

- supplierStore account (Admin profile) :=> (Accounts id, supplierStore id, ( Taken from accounts => name, email, password, created on, updated on) )

- SupplierEmployee account (Manager Account) :=> (Accounts id, SupplierEmployee id, supplierStore id, adminApproved?, ( Taken from accounts => name, email, password, created on, updated on) )

- Users accounts :=> (Accounts Id, User id,  Taken from accounts => (name, email, password, created on, updated on))


## Profile

- supplierStore profile :=> (supplierStore id, name, email, phone, geolocation, description, restrictions, created on, updated on)

- User profile :=> (1-1 with users account, phone, created on, updated on)


## Subscription Handling

- SupplierStore-Users :=> (id, supplierStore id, user id, created on) Many-Many relation between supplierStores and users


## Deals/Items

- Items :=> (item id, supplierStore id, name, type, item deal expiration date, stock available, description, restriction, created on, updated on) One store can have many items

- Wishlist :=> (user id, tags, created on, updated on)
