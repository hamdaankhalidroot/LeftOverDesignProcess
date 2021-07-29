- Land on a landing page with CTA (Register or Sign-in)

- Registration click opens a form

- Form has 2 clickable options Provider or ProviderEmployee
  * Provider Form ( Provider Name, email (standard regex), password, confirm password (len 8), phone (10 ints), address (Self populated by google api) , type(food bank, grocery store restaurant) but for now can only select food bank,
    IncomeRestrictionPerMemeber (Drop down per thousand $) if type selected is food bank display this option )
  * Provider is alerted that they will be notified after our approval if success, else alert why failed
  * Can navigate back
  
  * ProviderEmployee Form ( Provider(provider dropdown),ProviderEmployee-Otp (created by Provider and handed to), email (standard regex) , first name (Alphabets only), last name (Alphabets only) , password, confirm password (len 8) )
  * Logs them in if success, else alert why failed and lets them try again
  * Can navigate back

- Providers have to wait for Super-Admin (us) approval

- Once approved they are notified and logged in
