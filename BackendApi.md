# API's

- Create Token
- Refresh Token

- C SupplierStore (Un-authenticated)
- R SupplierStore (Authenticated & Authorized only for Supplier Admin, Supplier Employee, Users)
- UD SupplierStore (Authenticated & Authorized SUPPLIER ADMIN GROUP RESTRICTED API)
- C SupplierStoreEmployees ( Un-Authenticated but needs Admin from SupplierStore to Approve/update)
- R SupplierStoreEmployees (Authenticated & Authorized for SupplierStore Admin)
- UD SupplierStoreEmployees (Authenticated & Authorized for SupplierStore Admin)

- C Users (Un-authenticated)
- R SupplierStore (Authenticated & Authorized for only for Supplier Admin, Supplier Employee, the Particular User)
- UD Users (Authenticated & Authorized for particular User only)

- R Items (Authenticated & Authorized for SupplierStoreEmployees or SupplierStore Admin or Users) 
- CUD Items (Authenticated & Authorized for SupplierStoreEmployees or SupplierStore Admin)
- CRUD User_Supplier (Authenticated Authorized User or SupplierStoreAdmin)
