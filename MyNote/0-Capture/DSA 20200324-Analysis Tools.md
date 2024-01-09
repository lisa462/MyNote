標籤 : #筆記卡 
出處：
https://www.youtube.com/watch?v=d-PDYIqg_Kc&list=PLXVfgk9fNX2Kda9rttSvGROCtRQ3Sb8bA&index=6
![[Analysis_Tools 1.pdf]]

1. Analysis Tools，目標是分析演算法的是否優秀，及有什麼缺點，便於程序員修正
2. 一般來說分析會按照兩大方向判斷：
    1. Time Complexity，演算法處理資料的速度(花費的時間)
    2. Space Complexity，演算法處理資料的使用的暫存(佔據的記憶體)
    3. 兩者都是越少越好
3. 經典案例：
    1. Space Complexity of Recursive List Summing 遞歸列表求和的空間複雜度
        1. 計算消耗的暫存
    2. Time Complexity of Matrix Addition **矩陣加法的時間複雜度**
        1. 計算消耗的時間： `P . rows .cols + (Q + S) . rows + T` 其中Q、T是常數，零散的邊角料~
    3. Rough Time Complexity of Matrix Addition 差不多**矩陣加法的時間複雜度 → 粗略的計算**