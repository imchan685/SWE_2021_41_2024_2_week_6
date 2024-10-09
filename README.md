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
  > #### Input code
  > ```python
  > docker exec <container_name> cat /etc/os-release
  > ```
  > With this input, we can get release information about __container__
  > #### Output
  > ```python
  > PRETTY_NAME="Ubuntu 24.04.1 LTS"
  > NAME="Ubuntu"
  > VERSION_ID="24.04"
  > VERSION="24.04.1 LTS (Noble Numbat)"
  > VERSION_CODENAME=noble
  > ID=ubuntu
  > ID_LIKE-debian
  > HOME_URL="https://www.ubuntu.com/" SUPPORT_URL="https://help.ubuntu.com/"
  > BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
  > PRIVACY POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
  > UBUNTU_CODENAME=noble
  > LOGO-ubuntu-logo
  > ```
  > Output explain about my container's os information.



  > #### Input code
  > ```python
  > docker exec <container_name> git --version
  > ```
  > With this input, we can get information about __git version installed in my container.__
  > #### Output
  > ```python
  > git version 2.43.0
  > ```
  > Output is git version installed.



  > #### Input code
  > ```python
  > docker exec <container_name> python3 --version
  > ```
  > With this input, we can get information about __python version installed in my container.__
  > #### Output
  > ```python
  > Python 3.12.3
  > ```
  > Output is python version installed.



  > #### Input code
  > ```python
  > docker inspect --format="{{ .HostConfig.Binds }}" <container_name>
  > ```
  > With this input, we can check __mount directory of my container.__
  > #### Output
  > ```python
  > [./ossp_host_dir:/mnt/ossp_container_dir]
  > ```
  > Output is mount directory in my container.

  
