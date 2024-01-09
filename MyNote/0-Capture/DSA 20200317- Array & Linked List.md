標籤 : #筆記卡 
出處：
https://www.youtube.com/watch?v=B0ywTK-Lklw&list=PLXVfgk9fNX2Kda9rttSvGROCtRQ3Sb8bA&index=5
## Array 陣列

- **Ordered Array 指令陣列**
    - `insert` of ordered Array
    - Definition of ordered Array
        - 有特定順序的陣列
    - `update` and `remove` of ordered Array
    - `construct` of ordered Array
    - **Application : Book search within (Digital) Library**
        - selection sort. 選擇分類 → ex: `getMinIndex` multiple times
        - insertion sort. 插入分類
    - 兩種搜索方法：
        - **Sequential search Algorithm(從頭開始找)**
        - **Binary search Algorithm(從中間開始找→ 偷吃步)**

### Linked List

- Linked List 連接清單
    - 陣列中有小紙條，指示當前事件結束後，下一個事件/前一個事件的位置
    - Application : polynomial Computation (微積分)
        - Solution 0：use `ordered array` on (exponent指數, coefficient係數)
        - Solution 1 : singly Linked List for Flexible Insertion → overhead of `next` ⇔ flexible `insertAfter`
- Doubly Linked list 雙連接清單
    - 同時刪除前一個和下一個
- Linked List for Spare Vector(備用向量)
    - Application: spare Vector in Scientific Computing → Polynomial : can be viewed as special case of spare vector → Vector : [0,2.5,0,3.5,0] → spare Vector : [2.5,3.5]，排除資料是0的數列 → number of non-zero*size(pairs)