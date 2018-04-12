You need to take a copy of the list and iterate over it first, or the iteration will fail with what may be unexpected results.

For example (depends on what type of list):
```
for tup in somelist[:]:
    etc....
```

An example:
```
>>> somelist = range(10)
>>> for x in somelist:
...     somelist.remove(x)
>>> somelist
[1, 3, 5, 7, 9]

>>> somelist = range(10)
>>> for x in somelist[:]:
...     somelist.remove(x)
>>> somelist
```

ref : https://stackoverflow.com/questions/1207406/how-to-remove-items-from-a-list-while-iterating?utm_medium=organic&utm_source=google_rich_qa&utm_campaign=google_rich_qa