# LRU-Cache
Implementation of LRU Cache

LRU is actually a family of caching algorithms.
Discards the least recently used items first. This algorithm requires keeping track of what was used when, which is expensive if one wants to make sure the algorithm always discards the least recently used item. General implementations of this technique require keeping "age bits" for cache-lines and track the "Least Recently Used" cache-line based on age-bits. In such an implementation, every time a cache-line is used, the age of all other cache-lines changes.

![my image](https://upload.wikimedia.org/wikipedia/commons/8/88/Lruexample.png)

In the above example once A B C D gets installed in the blocks with sequence numbers (Increment 1 for each new Access) and when E is accessed, it is a miss and it needs to be installed in one of the blocks. According to the LRU Algorithm, since A has the lowest Rank(A(0)), E will replace A.

In the second to last step, D is accessed and therefore the sequence number is updated.

Finally, F is accessed taking the place of B which had the lowest Rank(B(1)) at the moment.

Read more about LRU https://en.wikipedia.org/wiki/Cache_replacement_policies#LRU
