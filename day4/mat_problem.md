
Mr. Vincent works in a door mat manufacturing company. One day, he designed a new door mat with the following specifications:

Mat size must be N X M. ( N is an odd natural number, and M is 3 times N.)

```
# Enter your code here. Read input from STDIN. Print output to STDOUT
n, m = map(int, input().split())
pattern = [('.|.'*(2 * i + 1)).center(m,'-') for i in range(n//2)]
print('\n'.join(pattern + ['WELCOME'.center(m, '-')] + pattern[::-1]))
```
