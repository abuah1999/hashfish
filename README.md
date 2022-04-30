# hashfish

As an exercise, I implemented a new Hashtable class in python using this tutorial: [https://realpython.com/python-hash-table/](https://realpython.com/python-hash-table/).
It supports all of the CRUD operations:

1. Creation:

```
ht = Hashtable()
ht is None # --> False
```

2. Retrieval:

```
ht = Hashtable.from_dict({1:"Romeo", 2:"Benvolio", 3:"The Friar"})
ht[2] # --> "Benvolio"
```

3. Update:

```
ht[1] = "Rosalind"
ht[1] = "Juliet"
ht[1] is "Juliet" # --> "True"
```

4. Deletion:

```
ht[3] = "Mercutio"
del ht[3]
ht[3] # --> KeyError
```

The class also supports the ```len``` operator, ```print```, and string conversion. It makes use of closed addressing and dynamic resizing based on a calculation of the load factor in order to deal with collisions. 
It can return all keys, values, or items and maintains the insertion order.
