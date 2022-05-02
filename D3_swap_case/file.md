

Complete the swap_case function in the editor below.
swap_case has the following parameters:
string s: the string to modify
Returns
string: the modified string
Input Format

A single line containing a string .

---
def swap_case(s):
    dd = ("".join(i.lower() if i.isupper() else i.upper() for i in s))
    return dd 
    
if __name__ == '__main__':
    s = input()
    result = swap_case(s)
    print(result)
 ---
s.swapcase() can be used for operation
