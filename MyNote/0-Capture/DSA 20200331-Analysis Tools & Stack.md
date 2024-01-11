出自：[DSA 20200331: Analysis Tools / Stack (youtube.com)](https://www.youtube.com/watch?v=-1FYYVpgyUo&list=PLXVfgk9fNX2Kda9rttSvGROCtRQ3Sb8bA&index=7&t=1s)
Project：[[考上台大網媒所]]
# Analysis Tools
## Asymptotic Notations
目標：如何取得程式消耗的時間或空間的約略數字
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
* Analysis of Sequential Search
	* 一個一個找，花費
* Analysis of Binary Search
	* 從中間找，花費常數logN那麼多輪
* Sequential and Binary Search
* 設定Array 無排序有兩個選擇
	* Direct-SEQ-SEARCH(list,n,num)-O(n) time
		* 直接在陣列找，花費等同於陣列長度的時間
	* SORT-AND-BIN-SEARCH(list,n,num)-SEL-SORT and O(log n)
		* 先排序陣列，再用BIN函數找。花費排序時間+ BIN搜索的時間
	* Q 那麼要怎麼計算由包含兩個以上函數的所消耗的時間呢?
	* Q 如何計算多個big-o所花費的時間?
		* 定義，證明-影片時間 [01:](https://youtu.be/-1FYYVpgyUo?list=PLXVfgk9fNX2Kda9rttSvGROCtRQ3Sb8bA&t=6962)
		* Some Properties of Big-O
		* Big-O使一個小於大於的東東
		* Theorem(封閉律)![[Pasted image 20240111201751.png]]
		* Theorem(遞移律)![[Pasted image 20240111201758.png]]
		* Theorem(併吞律)![[Pasted image 20240111202213.png]]
			* 只會留下最大的項，秦國把六國吞併
			* 什麼是Big-O?如何定義?工具?如何操作?
			* 用行話來說為什麼N的演算法，N2平方的演算法
			* 比較花時間的項目是什麼?
### Combine


