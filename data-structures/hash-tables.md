# Hash Tables

It is probably the most useful data structure to solve coding problems, but you also use it all the time in real life as well. The author of CTCI, Gayle Laakmann McDowell, like to say:
> In fact one technique I often tell people is just, for any problem, have a hash table at the top of your mind as a possible technique to solve the problem.

It is composed by a map of a `key` to a `value` where the key is store using a hash function, thats why we almost the time have a O(1) tinme complexity to search, insert and delete.

<img src="../img/data-structure/hash-tables/hash_table.png" alt="hash table" width="400"/>

So, when created

## Time complexity in big O notation

| Algorithm  | Average  | Worst Case  |
| ---------- | -------- | ----------- |
|  Space     | O(n)     | O(n)        |
|  Search    | O(1)     | O(n)        |
|  Insert    | O(1)     | O(n)        |
|  Delete    | O(1)     | O(n)        |

## When there is the worst case?
The most common worst case scenario in hash is the hash collision problem. Hash collisions are practically unavoidable when hashing a random subset of a large set of possible keys. For example, if 2,450 keys are hashed into a million buckets, even with a perfectly uniform random distribution, according to the birthday problem there is approximately a 95% chance of at least two of the keys being hashed to the same slot.

Therefore, almost all hash table implementations have some collision resolution strategy to handle such events. Some common strategies are described below. All these methods require that the keys (or pointers to them) be stored in the table, together with the associated values.

But for the most problems in code challenges we generally talk about constant time.

## TODO
* Handling collisions;
* How hash tables grow/shrink;
* Implementing a simple hash table;

---
* The reference to this file is the page 88.
* [Wikipedia page for hash table](https://en.wikipedia.org/wiki/Hash_table#Collision_resolution)
* Video Explaning hash tables by HackerRank with Gayle Laakmann McDowell.

[![https://img.youtube.com/vi/shs0KM3wKv8/0.jpg](https://img.youtube.com/vi/shs0KM3wKv8/0.jpg)](http://www.youtube.com/watch?v=shs0KM3wKv8)
