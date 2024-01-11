出自：[DSA 20200331: Analysis Tools / Stack (youtube.com)](https://www.youtube.com/watch?v=-1FYYVpgyUo&list=PLXVfgk9fNX2Kda9rttSvGROCtRQ3Sb8bA&index=7&t=1s)
# Analysis Tools
## Asymptotic Notations
目標：如何取得程式消耗的時間或空間的約落數字
### Rough Upper Bound
目的，證明兩個程式的性質的方法
**big-O** : arguably the most used "language" for complexity.

方法1：**More Intuitions on Big-O** : *如果f(n)/g(n)的極限值小於c,證明f(n)這個函式比g(n)更小或更慢。*
*該處要應用到微積分的極限值，當n無限大時，f(n)和g(n)的回應。*
* 他跑的比裡面的函數慢或是差不多
* 他在函數中建立排序
* 比較小的項，會被忽略，只會留下主要項
方法2：**Formal Definition of Big-O***兩個相除的結果是否相等，設立假設函數是大於零，是整數等...以最接近的值，做更好的限制*。*優點：沒有收斂也能使用*
![[Pasted image 20240111183937.png]]

**limit Intuition => formal Definition**
![[Pasted image 20240111184038.png]]
F/g 約小於等於 c
目標是什麼? -> 出現n0
若n比n0，f <= c' * g (c',n') 為ture 
	則 f(n) = O(g(n))
想法：
* 透過微分極限收斂(more intuition)或是找圖形天花板(Formal Definition)的方法，比較兩個函數的**粗略**的成效。
* 注意，這是一個證明題目。



### Definitions
設n >=0
* omega-下限
* big-o-上限
* semilar-上限+下限
  The Seven Functins as *g * 7個常用範例函數*
* 
