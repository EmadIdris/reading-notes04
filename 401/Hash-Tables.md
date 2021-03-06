# What is a Hashtable?

![](https://upload.wikimedia.org/wikipedia/commons/thumb/7/7d/Hash_table_3_1_1_0_1_0_0_SP.svg/1200px-Hash_table_3_1_1_0_1_0_0_SP.svg.png)

**Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.**

**Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.**
**Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.**

# Why do we use them?


1- Hold unique values
2- Dictionary
3- Library

# What Are they

**Hashtables are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value.**

**The basic idea of a hashtable is the ability to store the key into this data structure, and quickly retrieve the value. This is done through what we call a hash. A hash is the ability to encode the key that will eventually map to a specific location in the data structure that we can look at directly to retrieve the value.**

**Since we are able to hash our key and determine the exact location where our value is stored, we can do a lookup in an O(1) time complexity. This is ideal when quick lookups are required.**

## Example :
![](https://www.researchgate.net/profile/Erin-Hastings/publication/228958917/figure/fig1/AS:340199050629120@1458121182977/An-example-of-mobile-objects-in-a-grid-a-hash-table-and-the-object-index.png)
["Greenwood:98103", "Downtown:98101", "Alki Beach:98116", "Bainbridge Island:98110", ...] 