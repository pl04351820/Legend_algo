### Find duplicate numbers in a array (there maybe be many duplicate number and duplicate many times)
- Sort algorithm 
    Sort first, then travesal from begin to end
    Time: O(nlog(n)) Space: O(1)

- Hashtable
    Store every number in hashtable
    Time: O(n)  Space:O(n)

- If the array is [0, 1, ... , n] sequence, we can try to do something same as bucket sort.
    Iterate the array, put the value into relevant index. 
    Ex: [2, 3, 1, 0, 2, 5, 3]
    [1, 3, 2, 0, 2, 5, 3]
    [3, 1, 2, 0, 2, 5, 3]
    [0, 1, 2, 3, 2, 5, 3] Return True
    Time: O(n) (everynode at most transfer 2 times). Space: O(1)

- In place, no change element and only Find True or False and one duplicate number.
    Binary count. Divide arr in binary method.
    [2, 3, 5, 4, 3, 2, 6, 7].  8 / 2 = 4
    1 ~ 4 : 5 
    5 ~ 7 : 3
    Which means 1 ~ 4 dupilicate.  4 / 2 = 2
    1 ~ 2 : 2
    3 ~ 4 : 3       
    Which means 3 ~ 4 duplicate. 2 + 2 / 2 = 3
    3: 2
    4: 1
    3 is duplicate and return 3.
    Time: O(nlogn)  Space: O(1)  No change the structure of array.


    