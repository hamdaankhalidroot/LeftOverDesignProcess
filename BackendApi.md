# API's

- Create Token
- Refresh Token

- C SupplierStore (Un-authenticated)
- R SupplierStore (Authenticated only for Supplier Admin, Supplier Employee, Users)
- UD SupplierStore (SUPPLIER ADMIN GROUP RESTRICTED API)
- C SupplierStoreEmployees ( Un-Authenticated but needs Admin from SupplierStore to Approve/update)
- R SupplierStoreEmployees (Authenticated SupplierStore Admin)
- UD SupplierStoreEmployees (Authenticated SupplierStore Admin)

- C Users (Un-authenticated)
- R SupplierStore (Authenticated only for Supplier Admin, Supplier Employee, the Particular User)
- UD Users (Authenticated particular User only)

- R Items (Authenticated SupplierStoreEmployees or SupplierStore Admin or Users) 
- CUD Items (Authenticated SupplierStoreEmployees or SupplierStore Admin)
- CRUD User_Supplier (Authenticated Authorized User or SupplierStoreAdmin)
