# Readings: CRUD

1. In your own words, describe what each group of status code represents:
  - 100’s
    - used to send information to the client
  - 200’s
    - success codes: used to tell the client that all validation requirements are valid.
      - does not necessarily mean the request was successfully processed
  - 300’s
    - redirect codes: used to inform the client that what they are looking for has been moved
  - 400’s = error codes: used to inform the client that there is something wrong with the input on their end
  - 500’s = server error codes: used to inform the client that something went wrong on the server's end
2. What is a status code 202?
  - Accepted: often used for async processing, used to inform the client that a request was valid but still being processed
3. What is a status code 308?
  - Permanent Redirect: used to inform the client that a resource will be available at a new URL
4. What code would you use if an update didn’t return data to a client?
  - 204: No Content
5. What code would you use if a resource used to exist but no longer does?
  - 410: Gone
6. What is the ‘Forbidden’ status code?
  - 403 Forbidden: Client does not have permissions to access the resource.
