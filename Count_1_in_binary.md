# Count how many 1 in binary representation structure.
- Iterate every bits
```python
    while n:
        if n & 1:
            count += 1
        n = n >> 1
```
- & whole number
The idea is (n-1) & n will change the first 1 to 0. Counting from right to left.
```python
    while n:
        count += 1
        n = (n-1) & n
```