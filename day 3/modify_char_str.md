### Task
Read a given string, change the character at a given index and then print the modified string.
### Complete the mutate_string function in the editor below.

mutate_string has the following parameters:
string string: the string to change
int position: the index to insert the character at
string character: the character to insert
string: the altered string

```
def mutate_string(string, position, character):
    return string[:position] + character + string[(position + 1):]

if __name__ == '__main__':
    s = input()
    i, c = input().split()
    s_new = mutate_string(s, int(i), c)
    print(s_new)
```
