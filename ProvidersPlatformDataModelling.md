# Models and Relations

### Accounts
- id PK
- email
- hashed password
- Type (Provider, Shopper)

### Provider Profile Model
- Provider_Id PK
- name String
- type (Food Bank, Grocery Store , Restaurant)
- address String
- email String
- phone_num Int
- approved_by_super_admin Boolean
- created_on Timestamp
- updated_on Timestamp

### ProviderEmployee Profile Model -> (The employee that creates a Provider has admin credentials by default true is_admin :) )
- provider_employee_id PK/FK from Accounts (one-one from accounts) 
- provider_id FK
- is_admin
- first name String
- last name String
- created_on Timestamp
- updated_on Timestamp

### OTP-New-Provider-Employee (ProviderEmployee of admin type can publish OTP's for employees to signup)
- otp_id PK
- otp_value String (Random uid that is created)
- ProviderId FK
- published_at TimeStamp
- CreatedBy-ProviderEmployeeId
- expiring_at TimeStamp
- used Boolean

### item (stores item id to type)
- item_id Pk to food_bank_item
- Type (food_bank_item, grocery_store_item, restaurant_item)

### food_bank_item (posted by providers of the type food bank only)
- item_id FK to item
- ProviderId FK
- CreatedBy-ProviderEmployeeId FK Null if created by providerId admin
- UpdatedBy-ProviderEmployeeId FK Null if created by providerId admin
- UnpublishedBy-ProviderEmployeeId FK Null if noitfy created by providerId admin
- name String
- description String
- units Int
- amount_restriction Int
- Published Boolean
- created_on Timestamp
- updated_on Timestamp
