<b>Book</b>: Leetcode 101

<b>Address</b>: https://github.com/changgyhub/leetcode_101/blob/master/LeetCode%20101%20-%20A%20LeetCode%20Grinding%20Guide%20(C%2B%2B%20Version).pdf

<b>目录</b>

<b>第一章 题目分类</b>

<b>第二章 最易懂的贪心算法</b>

<b>第三章 玩转双指针</b>

<b>第四章 居合斩！二分查找</b>

<b>第五章 千奇百怪的排序算法</b>

<b>第六章 一切皆可搜索</b>

<b>第七章 深入浅出动态规划</b>

<b>第八章 化繁为简的分治法</b>

<b>第九章 巧解数学问题</b>

<b>第十章 神奇的位运算</b>

<b>第十一章 妙用数据结构</b>

<b>第十二章 令人头大的字符串</b>

<b>第十三章 指针三剑客之一：链表</b>

<b>第十四章 指针三剑客之二：树</b>

<b>第十五章 指针三剑客之三：图</b>

<b>第十六章 更加复杂的数据结构</b>

<b>第十七章 后记</b>

---

<b>Aug 05, 2021</b>

0. 第一章 题目分类 & 第二章 最易懂的贪心算法
1. ![常见题型](https://github.com/tinghe14/STUDY-LeetCode-Python-Note/blob/main/Book_Leetcode_101/%E5%B8%B8%E8%A7%81%E9%A2%98%E5%9E%8B.png)
2. 分类：第一大类是算法。本书从最简单的贪心算法讲起，然后逐渐到二分查找，排序算法和搜索算法，最后是难度比较高的动态规划和分治算法；第二大类是数学，包括纯数学的数学问题，和偏向计算机知识的位运算问题。这类问题通常测试是否聪敏，在实际工作中并不常用，建议可以优先精力放在其他大类上；第三大类是数据结构，包括c++ stl内包含的常见数据结构，字符串处理，链表，树和图。其中，链表，树和图都是指针表示的数据结构。最后我们也将介绍一些更加复杂的数据结构，比如经典的并查集和lRU.
3. 贪心算法

---

<b>Aug 17, 2021</b>

0. 第三章 玩转双指针
1. 算法解释：双指针主要用于遍历数组，两个指针指向不同元素，从而协同完成任务。也可以延伸到多个数组的多个指针。
    + 若两个指针指向同一个数组，遍历方向相同且不会相交，则也称为滑动窗口，经常用于区间搜索
    + 若两个指针指向同一个数组，遍历方向相反，则可以用来进行搜索，待搜索的数组往往是排好序的
2. 167 two sum II - input array is sorted (easy)
3. 88 merge sorted array (easy)
[88](https://github.com/tinghe14/STUDY-LeetCode-Python-Note/blob/main/Book_Leetcode_101/Pic/%E7%AC%AC%E4%B8%89%E7%AB%A0/88.png)
link: https://www.youtube.com/watch?v=ANUDq_2Bs04
4. 142 linked list cycle II (medium)
[142](https://github.com/tinghe14/STUDY-LeetCode-Python-Note/blob/main/Book_Leetcode_101/Pic/%E7%AC%AC%E4%B8%89%E7%AB%A0/142.png)
link: https://www.youtube.com/watch?v=9SD2ccDW5CY
5. 76 minimum window substring (hard)
??
link: https://www.youtube.com/watch?v=CX6_L9GLldU

---

<b>Sept 1, 2021</b>

0. 第四章 居合斩！二分查找
1. 算法解释： 二分查找也称为二分法，每次查找十将带查找区间分成两部分并只取一部分继续查找，将查找的复杂度大大减少。对于长度为o(n)的数组，二分查找的时间复杂度为o(logn)。比如，给定排序好的数组{3,4,5,6,7}，我们想查找4在不在这个数组内，第一次折半时考虑中位数5，以为5大于4，如果4在这个数组中，那么一定在5的左边，于是我们的查找区间变成[3,4,5]...以此，我们只进行了2次查找，如果是便利数组，最坏的情况则需要查找5次。
2. 69 Sqrt(x) (easy) solution: book p15/143 corner case?sqrt? 如何移动？牛顿迭代法？
3. 34 find first and last position of element in sorted array (medium) 
link: https://goodtecher.com/leetcode-34-find-first-and-last-position-of-element-in-sorted-array/
4. 81 search in rotated sorted array II (medium) 即使数组被旋转过，我们仍然可以利用这个数组的递增性，使用二分查找。对于当前的中点，如果它指向的值小于等于右端，那么说明右区间是排好序的；反之，那么说明左区间是排好序的。如果目标值位于排好序的区间内，我们可以对这个区间继续二分查找。

---

<b>Sept 14, 2021</b>

0. 第五章 千奇百怪的排序算法
1. 
