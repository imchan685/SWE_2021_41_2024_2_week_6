# SWE_2021_41_2024_2_week_6 

### Week 4 Assignment 

#### * Week 4 repository link
> [github](https://github.com/imchan685/SWE_2021_41_2024_2_week_4)

 #### + my code

   ```python
    def isHappy(n):
  arr = []
  while n != 1 and n not in arr:
    arr.append(n)
    summ = 0
    while n > 0:
      digit = n % 10
      summ += digit*digit
      n //= 10
    n = summ
  return n==1
  ```
  
