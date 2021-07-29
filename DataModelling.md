# Models and Relations

## Providers

### Provider Authentication Model
- provider_id PK
- name String
- type (grocery store, food bank, restaurant)
- address String
- email String
- phone_num Int
- approved_by_admin Boolean
- created_on Timestamp
- updated_on Timestamp

### ProviderEmployee Authentication Model
- provider_employee_i PK
- provider_id FK
- email String
- first name String
- last name String
- created_on Timestamp
- updated_on Timestamp

### OTP-Provider-Employee (Used to manage providers publishing OTP's for employees to signup)
- otp_id PK
- ProviderId FK
- published_at TimeStamp
- expiring_at TimeStamp
- used Boolean

### Provider (Food Bank Only) Item (posted by providers of the type food bank only)
- item_id PK
- ProviderId FK
- CreatedBy-ProviderEmployeeId FK (0) to noitfy created by providerId admin, -1 to notify it was by Super-admin
- UpdatedBy-ProviderEmployeeId FK (0) to noitfy created by providerId admin, -1 to notify it was by Super-admin
- UnpublishedBy-ProviderEmployeeId FK (0) to noitfy created by providerId admin, -1 to notify it was by Super-admin
- name String
- description String
- units Int
- amount_restriction Int
- Published Boolean
- created_on Timestamp
- updated_on Timestamp

## Users
TODO
