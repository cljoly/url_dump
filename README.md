# url_dump
POST urls, GET atom feed

## TODO

- `/user/<token>`
  - POST add link, title
  - GET return atom feed
- `/_*/*`: reserved
- command line client:
  - add user with token (multiple token per user if we want)
  - revoke token
- multi user: multiple sqlite databases
- sqlite tables:
  ```
  entries(title, url, created_by_token, addded_on)
  token(id, token_salted_hash, comment)
  ```
  
https://docs.rs/scrypt/0.5.0/scrypt/     
https://docs.rs/warp/0.2.5/warp/
