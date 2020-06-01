# Class 30 - Hashtables - 5/22/2020  

## Terminology
* Hash - the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In hash tables, it is used to determine the index of the array
* Buckets - data contained in each index of the array of the hashtable. Each index is a bucket and usually buckets are implemented in Linked List.
* Collisions - it happens when more than one key gets hashed to the same location of the hashtable

## Advantages of Hashtables
* Time complexity for adding a value is O(1)
* Time complexity for accesing/reading a value is O(1)

## What are Hashtables
* A data structure that utilize key value pairs
* Store the key into data structure and quickly retrieve the value through `hash`
* A `hash` is to encode the key that will eventually map to a specific location in the data structure that we can directly to retrieve the value
* Time complexity for looking up a value is O(1)

## Implementation
* Create an array with certain size
* Create a hash function and use it to produce an index for a given key-value pair
* Store the given key-value pair at index in the array  
  * If nothing stored at index in the array, then create a Linked List and add the given key-value pair to the head
  * Else, add the given key-value pair to the head