出處：
https://www.youtube.com/watch?v=pAs8Swu1Y3Y&list=PLXVfgk9fNX2Kda9rttSvGROCtRQ3Sb8bA&index=5&t=451s

_**Sparse Vector**_

- Real-World Usage of Sparse Vector : LIBSVM
    
- 說明(來自AI)
    
    Real-World Usage of Sparse Vector : LIBSVM” 是指在實際應用中使用 LIBSVM（一種支持向量機的庫）時，如何使用稀疏向量。在機器學習和數據科學中，稀疏向量是一種數據表示方法，其中大多數元素為零。LIBSVM 使用這種格式來節省存儲空間並提高計算效率1[2](https://www.csie.ntu.edu.tw/~cjlin/libsvm/faq.html)。
    
    [例如，一個稀疏向量可能看起來像這樣：](https://stackoverflow.com/questions/44965186/how-to-understand-the-format-type-of-libsvm-of-spark-mllib)`0 128:51 129:159 130:253 131:159 132:50`[。這裡，數字 `0` 是標籤或目標變量，`128:51`](https://stackoverflow.com/questions/44965186/how-to-understand-the-format-type-of-libsvm-of-spark-mllib) 表示索引為 128 的特徵其值為 51，以此類推。這種表示方法只需存儲非零元素，因此對於具有許多零元素的大型數據集非常有用
    
- 範例(來自AI)
    
    當然可以，以下是如何在 Python 中使用 `scipy` 庫創建和使用稀疏向量的示例：
    
    ```python
    from scipy.sparse import csr_matrix
    
    # 創建一個列表，其中每個子列表都是一個特徵向量
    data = [[1, 0, 0, 1, 0, 0], [0, 0, 2, 0, 0, 1], [0, 0, 0, 2, 0, 0]]
    
    # 將密集矩陣（列表的列表）轉換為稀疏矩陣
    sparse_data = csr_matrix(data)
    
    print(sparse_data)
    
    ```
    
    當您運行此代碼時，它將以 `(row, column) value` 的格式打印出稀疏矩陣。例如，`(0, 0) 1` 表示在矩陣的第一行和第一列，值為 1。這是存儲和處理大量包含許多零的矩陣的一種更有效的方式。
    
    請注意，這只是一個簡單的示例，實際的數據會更大且更複雜。另外，如果還未安裝 `scipy` 庫，請記得使用 pip 進行安裝：
    
    ```
    pip install scipy
    
    ```
    

範例：

- Linked List Reversal 鍊錶反轉
- “Cycle” in Linked List 鍊錶中的“循環”
- Middle of Linked List 鍊錶中間
- Tip : two pass. or **tortoise-hare(turtle-rabbit) algorithm**
    - 龜兔賽跑，設烏龜每次跑1步，兔子跑2步。因為兔子比烏龜快1步，所以：
        - 兔子若撞上烏龜，代表有“Cycle” in Linked List
        - 兔子跑完則烏龜剛好在路程的一半，故烏龜的位置就是Middle of Linked List.
        - 