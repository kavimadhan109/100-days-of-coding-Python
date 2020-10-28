## Given a list of numbers and a number k, return whether any two numbers from the list add up to k.

```
[10, 15, 3, 7] 
17
True

[10, 15, 3, 7]
5
False
```


```
def twosum(lst, k):
    for i in range(len(lst)):
        for j in range(len(lst)):
            if i != j and lst[i] + lst[j] == k:
                return True
    return False

lst1 = list(map(int,input().split(" ")))
kn = int(input())
print(twosum(lst1, kn))
```       
