# Basic web app security checklist

  - [ ] make sure that all traffic is encrypted (using tls & https)
  - [ ] hash all passwords in your database using bcrypt, so even if you get compromised it would take more than a lifetime with supercomputers to decrypt the passwords for logging in
  - [ ] do not have the decryption key close to your sensitive data (e.g. both in the same database)
  - [ ] rate limit actions (e.g. you should be restricted for some time if you have more than 5 login attempts per minute)
  - [ ] check on server (& maybe client) if the user shall be able to perform a specific operation.
  - [ ] log security breaches
  - [ ] maybe allow only one session per user at a given time (login on another system -> loose login on another system)
  
# Advanced

  - [ ] add two factor authentication
  - [ ] log every move of every user
