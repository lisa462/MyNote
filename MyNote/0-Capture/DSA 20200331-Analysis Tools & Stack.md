出自：[DSA 20200331: Analysis Tools / Stack (youtube.com)](https://www.youtube.com/watch?v=-1FYYVpgyUo&list=PLXVfgk9fNX2Kda9rttSvGROCtRQ3Sb8bA&index=7&t=1s)
# Analysis Tools
## Asymptotic Notations
目標：如何取得程式消耗的時間或空間的約落數字
### Rough Upper Bound
目的，證明兩個程式的性質的方法
**big-O** : arguably the most used "language" for complexity.
**More Intuitions on Big-O**：
他跑的比裡面的函數慢或是差不多
他在函數中建立排序
比較小的項，會被忽略，只會留下主要項
缺點：必須存在極限(微積分收斂)
**Formal Definition of Big-O**：兩個相除的結果是否相等，設立假設函數是大於零，是整數等...
以最接近的值，做更好的限制
優點：沒有極限也能使用
![[Pasted image 20240111183937.png]]

**limit Intuition => formal Definition**
![[Pasted image 20240111184038.png]]
F/g 約小於等於 c
目標是什麼? 出現