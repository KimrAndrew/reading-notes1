# Authentication

1. What is OAuth?
  - OAuth is an open-standard authorization protocol or framework that descripbes how unrelated servers and services can safely allow authenticated access to hteir assets without actually sharing the initial related, single logon credential.
2. Give an example of what using OAuth would look like.
  - logging into another website using your google account
3. How does OAuth work? What are the steps that it takes to authenticate the user?

  1. first website connects to the second website using OAuth, providing the user's verified identity
  2. second site generates a on-time token and a onetime secret unique to that transaction
  3. first site gives this token and secret to the user's client software
  4. clients software requests token and secret to the authorization provider
  5. user may be asked to authenticate by second site
  6. user/client software approves a transaction
  7. user is given an approved access token
  8. user gives approved access token to first website
  9. first website gives the access token to second website as proof of authentication
  10. second website lets the first website access their site on behalf of the user
  11. user sees a successful transaction occur
  12. what makes 0Auth special is its wide adoption and ability to work across the web
4. What is OpenID
  - OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans
