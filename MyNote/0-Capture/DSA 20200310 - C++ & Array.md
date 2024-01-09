標籤 : #筆記卡 
出處：
https://www.youtube.com/watch?v=1yyu70Vy9Zc&list=PLXVfgk9fNX2Kda9rttSvGROCtRQ3Sb8bA&index=4
### From C to C++

**C語言和C++語言的5種好用的不同**

|項目|說明|
|---|---|
|Reference vs. “pointer”|Reference : C++way of smart/safer “pointer”|
|Class vs. Structure|Class : C++way of structure “with action”|
|Operator vs. Function|Operator overloading : C++way of programming with (some) complicated(編譯) class more easily.|
|Template vs. Copy/paste|template : C++ way of automating safer copy/paste by complies.|
|Standard Template Library in C++(縮寫STL)|one data structure/algorithm can be applied to many classes.|

### Array

- Array : numbered lockers (數值+位置)
- desired property : fast computation of address. → fast random access.
    - access(get 獲得) - maintain (update 更新、維護)
- implicit assumption(隱式假設) : `Index` to address done by fast math formula.
- STL vector(向量) : a more “structure” way of using array.
    - `insertByIndex(index,data)`
    - `insertAtBach(data)`

### Two Dimensional Array 二維陣列

- 取位置的方法
    1. one block (better and [succinct](https://dictionary.cambridge.org/zht/%E8%A9%9E%E5%85%B8/%E8%8B%B1%E8%AA%9E-%E6%BC%A2%E8%AA%9E-%E7%B9%81%E9%AB%94/succinct) 簡潔) - 快速
    2. Array of arrays (perfume) - 好記
- Knowing architecture helps
    - row sum (Faster) vs. column sum
    - Reason : 底層的硬體搜索的設計，使得Row sum 更快速，因為能抓到更多的資料。兩者差距約2倍

### Ordered Array

- an array of consecutive elements with ordered values.
    - 有東西的櫃子拍按照特定順序，排在最前方。