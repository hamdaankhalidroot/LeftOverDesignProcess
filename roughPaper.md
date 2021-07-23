SupplierStore have attributes like phone num, email, address, and deals.
SupplierEmployees have access to SupplierStore and can managge SupplierStore's Attribute's

SupplierStore (SupplierStoreId, name, phone, email, street, city, state, zipcode, geohash)
SupplierEmployees (SupplierEmployeeId, type(admin or manager), email, password)

EmployeeToSupplier (SupplierEmployee id, SupplierStore id)


