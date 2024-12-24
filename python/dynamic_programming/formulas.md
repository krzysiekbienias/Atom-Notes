# Applying memoaization
Memoaization is top - down approach 
Memoaization in leyman terms meaning checking if we didn't solve the subproblem before.
In practice we need lookup table that is dictionary created inside function like following:

``` python
lookup={} if lookup is None else lookup
```

and we need this lookup also have as additional parameter of function for instance 
```python 
def fib(n,lookup=None):
    lookup={} if lookup is None else lookup
     
```
# House robber
$$rob(i)=\left\{\begin{array} {rl} 0 & i\ge len(arr)\\ 
max(arr[i]+rob(i+2),rob(i+1)) & i < len(arr) \end{array} \right.$$

# Ways to climb
$$ways(n)=\left\{\begin{array} {rl} 1 & n=0 \\ 
0 & n<0 \\
\sum_{\substack{jump \in \text{jumps}}}ways(n-jumps)& otherwise \end{array} \right.$$


$$\sum_{\substack{jump \in \text{jumps}}}$$