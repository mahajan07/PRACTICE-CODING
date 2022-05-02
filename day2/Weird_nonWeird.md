Given an integer, , perform the following conditional actions:

If  is odd, print Weird
If  is even and in the inclusive range of 2 to 5, print Not Weird
If  is even and in the inclusive range of 6 to 20 , print Weird
If  is even and greater than , print Not Weird


### CODE
#!/bin/python3

import math
import os
import random
import re
import sys



if __name__ == '__main__':
    n = int(input().strip())
    if (n in range(6,21) or n%2 != 0):
        print("Weird") 
    else:
        print("Not Weird")
