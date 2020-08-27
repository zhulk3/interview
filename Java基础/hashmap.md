hashmap是一个用于存储key-value键值对的集合，每一个键值对也叫一个Entry这些Entry分散存储在一个数组中，使用hash算法确定每一个Entry的存储位置，如果出现hash冲突，就使用拉链法解决冲突。

默认初始长度16，设定长度为2的幂，扩容为2倍；

使用的hash算法，hash=hashCode(key)&length-1;length-1的二进制都是1，与运算的结果只与hashCode的最后几位有关，只要hashCode足够均匀，计算出的hash值就足够均匀；

Entry是HashMap的一个内部类，包括的数据成员有key、value、next，hash等；

hashMap在负载因子*数组长度大于等于当前hashMap的值以后会进行扩容，扩容分为两步，首先新建一个长度为当前数组长度两倍的数组，然后对每个对象重新hash，但是多线程如果同时扩容的话会出现链表环；



