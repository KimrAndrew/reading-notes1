# Hashtables

## What are they?

- use key/value pairs - every `Node`/`Bucket` has a key and a value
- keys are `hashed`, values can be accessed using this `hash` key to access values with a lookup of O(1)
- `hash` function takes a key and returns an integer

## Structure

### Hashing

- a hash code turns a key into an iteger
- output is determined only by their input
- should never involve any randomess
- same key should always return the same hash

### Creating a Hash

Suggestions for hash methods

- multiply all ASCII values together
- multiply it by a prime number
- use modulo to get the remainder when divided by the size of the array
- insert into the array at that index

### Collisions

What happens if two keys resolve to the same index? This is called a **collision**

- solved by initializing the empty indexes in the array as a `LinkedList`
