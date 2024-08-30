# Binary Search
🍇 對一個有序數組進行二分搜尋 {1,8, 10, 89, 1000, 1234} ，輸入一個數看看該數組是否存在此數，並且求出索引，如果沒有就提示"沒有這個數"。
留言

思路
首先確定該陣列的中間索引 mid = (left + right) /2
然後讓需要搜尋的數 findVal 和 arr[mid] 比較
2.1 findVal > arr[mid] ，說明要搜尋的數在mid右邊，因此需要遞迴的向右搜尋。
2.2 findVal < arr[mid] ，說明要搜尋的數在mid左邊，因此需要遞迴的向左搜尋。
2.3 findVal == arr[mid]，說明找到，就返回。
