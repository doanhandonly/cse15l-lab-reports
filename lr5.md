# **Lab Report 5**
# **Part 1 - Debugging Scenario**
![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/bd8f6dbb-04f5-4c8e-a3c4-bd2764a668ce)
![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/75f6b77a-0755-41db-8a41-c03ceb283b87)
![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/7727b4b5-d576-4b30-af91-6ca833f28a9d)
![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/1efbc4c3-f818-4eda-b4c3-51b96212dd2d)
Current working directory: 

![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/afb54cf5-5338-45d2-9c51-70703e19235e)


TA's Response:
 Hello, thanks for the VERY detailed response. I suggest you looking at places where you called size and start from there. (Try looking up what -- actually does).

![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/db5434b6-1334-4c6a-8293-3fe0b272316c)
![image](https://github.com/doanhandonly/cse15l-lab-reports/assets/127058698/6b7d8eb1-7acf-4809-90d6-e91a407051d0)

The bug was that I was using -- instead of - 1. -- decrements a value by one, and saving it. For example if num = 2, and I called num--, calling num again would return 1 instead of 2. I just needed to use the position of size - 1 to set that as the index of the rear value, but instead of using size - 1, I used size--, changing size in the process. That is why size was changed even though expandCapacity should not have affected the size at all. 

# **Part 2 - Reflection**
