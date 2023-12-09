# leetcode-train
**查找表**
链接：https://leetcode.cn/problems/two-sum/
思路：
1、用for暴力循环。空间复杂度小，但时间复杂度要o(n*n)
2、用哈希表。只遍历一次数组，每一次遍历，先计算出差值，然年在map中查找是否有这个差值，有则输出结果。没有则把这个遍历值加入map，便于后续继续比对。【为啥用map，不用数组=》首先，我们需要的是用值当key，然后key对应值存数组下标。数组和map都能满足，但如果数值过大，数组就会很大，空间复杂度就会很大；明显map没有这个问题。】
笔记：
map用法
let xxx = new Map([[key1, value1][key2, value2]]);
xxx.has(key)
xxx.get(key)
xxx.set(key, value)
