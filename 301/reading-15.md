# Web Request Response Cycle

## Client Sends an Http Request
  - url string 
  - common requests include
    - GET
    - POST
    - PUT
    - DELETE

## Server Recieves the Https Request
  - request can have:
    - params
    - queries
    - body
  - performs the functionality that matches the route of the request

## Server Sends Back a Response
  - response has a status and a body
    - status gives back information about how the server handled the request
      - 100: Information Responses
      - 200: Successful Responses
      - 300: Redirect Message
      - 400: Client Error Responses
      - 500: Server Error Responses
