# SWE_2021_41_2024_2_week_6 

### Week 4 Assignment 

* #### Week 4 repository link
  > [github](https://github.com/imchan685/SWE_2021_41_2024_2_week_4)

+ ####  My code

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
- #### Code description
  > In the inner __while__ loop, add the result value of __n%10__ to the __summ__. Then divide __n__ by 10.  
  > Continue until __n__ is below __0__.  
  > Append the resulting __summ__ value to __arr__ and replace the value of __n__ with __summ__.  
  > If there is a value equal to __n__ in __arr__, end the __while__ loop and return __false__ because it means you are <U>looping between several numbers.</U>  
  > Alternatively, if __n = 1__, return __true__ because the number entered means __happy number__.  

  ---
  ### Week 5 Assignment
  > #### input code
  > ```ubuntu
  > docker exec <container_name> cat /etc/os-release
  > ```
  > With this input, we can get release information about __container__
