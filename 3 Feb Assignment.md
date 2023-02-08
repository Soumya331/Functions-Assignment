Ans 1) def() is used to create a function.


```python
##function that returns list of odd numbers in the range of 1 to 25. 
def test1():
    for i in range(1,25,2):
        print (i)
test1()
```

    1
    3
    5
    7
    9
    11
    13
    15
    17
    19
    21
    23


Ans 2) *args and **kwargs are used when we are unsure about the number of arguments to pass in the functions.
## *args
def list(*num):
    product = 1
    
    for n in num:
        product*=n
    return product
    print("Product:",list(4,9,8,45))
    
## **kwargs
def sentence(**words):
    sentence = ''

    for words in words.values():
        sentence+=word
    return sentence
    
print("Sentence",sentence(a='Hello',b='Everyone'))



Ans 3) Iterator in Python is an object that is used to iterate over iterable objects like lists, tuples, dicts, and sets. 
The method used to initialise the iterator object and the method used for iteration are iter() and next() respectively.


```python
list = [2, 4, 6, 8, 10, 12, 14, 16, 18, 20]
iter1 = iter(list)
print(next(iter1))
print(iter1.__next__())
print(next(iter1))
print(next(iter1))
print(next(iter1))

```

    2
    4
    6
    8
    10


Ans 4)A generator is a function that returns an iterator that produces a sequence of values when iterated over.
Generators are useful when we want to produce a large sequence of values, but we don't want to store all of them in memory at once.

Yield keyword is used to create a generator function. A type of function that is memory efficient and can be used like an iterator object.

Eg) def all_even():
    n = 0
    while True:
        yield n
        n += 2

Ans5)
```python
def genprimes(limit): 
                     
    D = {}           
    q = 2

    while q <= limit:
        if q not in D:
            yield q
            D[q * q] = [q]
        else:
            for p in D[q]:
                D.setdefault(p + q, []).append(p)
            del D[q]
        q += 1

p = genprimes(1000)
prms = [i for i in p]

print (prms)
```

    [2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89, 97, 101, 103, 107, 109, 113, 127, 131, 137, 139, 149, 151, 157, 163, 167, 173, 179, 181, 191, 193, 197, 199, 211, 223, 227, 229, 233, 239, 241, 251, 257, 263, 269, 271, 277, 281, 283, 293, 307, 311, 313, 317, 331, 337, 347, 349, 353, 359, 367, 373, 379, 383, 389, 397, 401, 409, 419, 421, 431, 433, 439, 443, 449, 457, 461, 463, 467, 479, 487, 491, 499, 503, 509, 521, 523, 541, 547, 557, 563, 569, 571, 577, 587, 593, 599, 601, 607, 613, 617, 619, 631, 641, 643, 647, 653, 659, 661, 673, 677, 683, 691, 701, 709, 719, 727, 733, 739, 743, 751, 757, 761, 769, 773, 787, 797, 809, 811, 821, 823, 827, 829, 839, 853, 857, 859, 863, 877, 881, 883, 887, 907, 911, 919, 929, 937, 941, 947, 953, 967, 971, 977, 983, 991, 997]



```python
list = [2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71]
iter1 = iter(list)
print(next(iter1))
print(next(iter1))
print(next(iter1))
print(next(iter1))
print(next(iter1))
print(next(iter1))
print(next(iter1))
print(next(iter1))
print(next(iter1))
print(next(iter1))
print(next(iter1))
print(next(iter1))
print(next(iter1))
print(next(iter1))
print(next(iter1))
print(next(iter1))
print(next(iter1))
print(next(iter1))
print(next(iter1))
print(next(iter1))
```

    2
    3
    5
    7
    11
    13
    17
    19
    23
    29
    31
    37
    41
    43
    47
    53
    59
    61
    67
    71



```python

```


```python

```


```python

```


```python

```


```python

```

