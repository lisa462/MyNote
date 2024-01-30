> 取自：https://www.youtube.com/watch?v=8IOv2fnc01E
1. Introduction to Data Structures and Algorithms
2. What is Algorithms ? 
    1. 譜
    2. computation _n._ 計算;估計
3. [[Pseudo Code 虛擬碼]]
4. Introduction to Data Structures 介紹資料結構
5. why Data Structures and Algorithms
6. 簡單的程式

```c
// 在陣列Arry裡面，找到最小數值的位置。
int getMinIndex(int* arr, int len){
    int minpos = 0; int i;
    for(i = 1; i < len; i++){
        if(arr[i] < arr[minpos])
            minpos = i;
    }
    return minpos;
}

```

1. 資料結構較重視**程式（coding)、測試(test)和清除bug(debug )**的部分。


