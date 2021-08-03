- Post auth/login ( takes credentials returns jwt with user id & exp ) PUBLIC

- Post /provider/signup PUBLIC
- Get /provider/:id ( takes an id, and returns profile, and account info for the provider ) AUTHENTICATED
- Patch /provider/:id ( a provider can update their profile information ) AUTHENTICATED & AUTHORIZED ONLY FOR ADMIN PROVIDER OF THAT PARTICULAR ID
- DELETE /provider/:id ( a provider can update their profile information ) AUTHENTICATED & AUTHORIZED ONLY FOR SUPER_ADMIN
