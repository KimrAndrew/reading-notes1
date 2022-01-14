# Introduction to JSON Web Tokens

## What is JSON Web Token?

- open standard that defines a compact, self-contained way for securely transmitting information between parties
- digitally signed using a secret or public/private key pair
- signed tokens verify integrity of claims / encrypted tokens hide those claims

## When should you use JSON Web Tokens?

Authorization:
- most common scenario
- requests include the JWT once user is logged in

Information Exchange:
- good way of securely transmitting information
- can be sure senders are who they say they are

## What is the JSON Web Token structure?

- Header
- Payload
- Signature

### Header
- typically consists of two parts:
  - type of token
  - signing algorith

### Payload

- contains the claims
- three types of claims:
  1. registered
  2. public
  3. private
- Registered Claims:
  - provide a set of useful, interoperable claims
- Public claims:
  - can be defined at will by those using JWTs
- Private claims
  - custom claims created to share information

### Signature

- signature is used to verify the message wan't changed along the way
- can also verify that the sender is who it says it is
