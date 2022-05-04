
Given an integer, , print the following values for each integer  from 1 to n :

Decimal
Octal
Hexadecimal (capitalized)
Binary
The four values must be printed on a single line in the order specified above for each  from 1 to n .
Each value should be space-padded to match the width of the binary value of  and the values should be separated by a single space.
```
def print_formatted(number):
    l1 = len(bin(number)[2:])

    for i in range(1,number+1):
        print(str(i).rjust(l1,' '),end=" ")
        print(oct(i)[2:].rjust(l1,' '),end=" ")
        print(((hex(i)[2:]).upper()).rjust(l1,' '),end=" ")
        print(bin(i)[2:].rjust(l1,' '),end=" ")
        print("")
    
    
    # your code goes here

if __name__ == '__main__':
    n = int(input())
    print_formatted(n)
```
