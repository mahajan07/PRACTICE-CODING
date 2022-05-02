#### Print_full_name has the following parameters:
"""
string first: the first name
string last: the last name
Prints

string: 'Hello  firstname lastname! You just delved into python.'
Input Format. The first line contains the first name, and the second line contains the last name.
"""


```
# Complete the 'print_full_name' function below.
# The function is expected to return a STRING.
# The function accepts following parameters:
#  1. STRING first
#  2. STRING last

def print_full_name(first, last):
    # Write your code here
    print("Hello " + first + " "+ last + "!" + " You just delved into python.")
    
if __name__ == '__main__':
    first_name = input()
    last_name = input()
    print_full_name(first_name, last_name)

```