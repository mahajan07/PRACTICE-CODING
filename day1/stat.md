# Question
You are given an array of N integers separated by spaces, all in one line.

Display the following:
* Mean (m): The average of all the integers.

* Median of this array: In case, the number of integers is odd, the middle element; else, the average of the middle two elements.

* Mode: The element(s) which occurs most frequently. If multiple elements satisfy this criteria, display the numerically smallest one.

* Standard Deviation (SD).
SD = (((x1-m)2+(x2-m)2+(x3-m)2+(x4-m)2+...(xN-m)2))/N)0.5

where xi is the ith element of the array

* Lower and Upper Boundary of the 95% Confidence Interval for the mean, separated by a space. This might be a new term to some. However, it is an important concept with a simple, formulaic solution. 


# SOLUTION:
import pandas as pd
import numpy as np
from scipy import stats

n = int(input())
a = np.array(input().split())
a = a.astype(np.int32)

mean = np.mean(a)
sigma = np.std(a)
medi = np.median(a)
mod = stats.mode(a)
ci = stats.norm.interval(0.950004, loc=mean, scale=sigma/np.sqrt(n))
print("%.1f"%mean)
print("%.1f"%medi)
print("%.0f"%mod[0][0])
print("%.1f"%sigma)
print("%.1f %.1f"%(ci[0],ci[1]))
