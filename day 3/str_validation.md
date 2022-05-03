
### Your task is to find out if the string  contains: alphanumeric characters, alphabetical characters, digits, lowercase and uppercase characters.

* Input Format >> A single line containing a string .

* Output Format

1. In the first line, print True if S has any alphanumeric characters. Otherwise, print False.
2. In the second line, print True if S has any alphabetical characters. Otherwise, print False.
3. In the third line, print True if S has any digits. Otherwise, print False.
4. In the fourth line, print True if S has any lowercase characters. Otherwise, print False.
5. In the fifth line, print True if S has any uppercase characters. Otherwise, print False.



```
if __name__ == '__main__':
    s = input()
    print(any(c.isalnum() for c in s))
    print(any(c.isalpha() for c in s))
    print(any(c.isdigit() for c in s))
    print(any(c.islower() for c in s))
    print(any(c.isupper() for c in s))
```
