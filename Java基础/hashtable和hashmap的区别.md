1、线程安全，hashmap不是线程安全的，hashtable是线程安全的，通过synchronized实现的，hashmap不是，但是性能更好；

2、hashmap允许key为Null，但是hashTable不允许；

3、继承结构不同，hashmap实现自map接口，hashTable继承Dictionary抽象类同时实现了Map接口；

4、初始化大小不同，hashMap默认初始化16，hashTable默认是11，扩容也不同，hashMap是原来的两倍，hashTable是原来的两倍+1；

5、计算哈希值也不同，hashTable是计算key的hashCode后再与table的lenth做模运算，hashMap计算key的hashCode后再与lenght-1做位运算。