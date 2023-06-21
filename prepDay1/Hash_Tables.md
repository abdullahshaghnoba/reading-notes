# Hash Table Data Structure

## Summary:
A hash table is a data structure that allows for efficient storage and retrieval of data by using a technique called hashing. Hash tables use an analogy of a large array of buckets, each containing a key-value pair. This structure enables fast insertion, deletion, and retrieval of data, making it suitable for a wide range of applications.

---

## Analogy:
Imagine a library where books are organized using a unique identifier called a call number. Each book has a specific location on a shelf based on its call number. In this analogy, the library is a hash table, the call numbers are the keys, and the books are the values. This system allows for quick access to books by looking up their call numbers.

---

## Detail Explanation:
In a hash table, each key is transformed into an index using a hash function. The hash function takes the key and performs a computation to generate a unique numeric value. This index corresponds to a specific location in the underlying array, known as a bucket. The bucket holds the key-value pair associated with the given key.

- WHY: The purpose of using a hash function is to distribute the keys evenly across the array, ensuring efficient data retrieval. This reduces the search time as it provides a direct path to the bucket that contains the desired data.

- WHAT: The hash function converts the key into a numeric value. It may involve performing mathematical operations or manipulating the key's characters to generate the hash code. The resulting hash code is used as an index to access the corresponding bucket in the array.

- HOW: The hash code obtained from the hash function can sometimes lead to collisions, where two different keys produce the same index. To handle collisions, hash tables employ various collision resolution techniques. One common approach is chaining, where each bucket stores a linked list of key-value pairs. If a collision occurs, new items are added to the linked list at the appropriate bucket.

---

## Example:

Let's consider a scenario where we want to store the contact information of people in a hash table using their names as keys. We can use the following steps:

1. Create an empty hash table.
2. Define a hash function that transforms the names into numeric hash codes.
3. Take a person's name and pass it through the hash function to obtain the hash code.
4. Use the hash code as an index to locate the bucket in the hash table.
5. If the bucket is empty, add the name and associated contact information as a key-value pair.
6. If the bucket is not empty, handle collisions by adding the new key-value pair to the linked list at the bucket.
7. Repeat steps 3-6 for each person's contact information.

---

## Vocabulary/Definition List:

- Hash Table: A data structure that uses hashing to store and retrieve data efficiently.
- Hash Function: A function that converts a key into a unique hash code.
- Bucket: A location in the hash table's underlying array that holds key-value pairs.
- Collision: A situation where two different keys produce the same hash code.
- Chaining: A collision resolution technique where each bucket contains a linked list of key-value pairs.

---

## Cheat Sheet:

- Hash tables are used for efficient storage and retrieval of data.
- They use a hash function to transform keys into unique hash codes.
- Hash codes are used as indices to access buckets in the hash table's array.
- Collisions can occur when different keys produce the same hash code.
- Collision resolution techniques, such as chaining, are used to handle collisions.

