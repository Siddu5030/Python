 ## 1).Document today’s class with proper explanation using markdown, comments, examples and code.


### Class

   A class is like a blueprint or template for creating objects in computer programming.
  
  Defines the properties and behaviors that the objects belonging to that class will have.

### Ascii values
 Here we have the some values for each and every character called 'ascii'. The characters that can be in the form of upper function and lower function of alphabets like, (A,B,C,D,...),(a,b,c,d,...).


```python
ord('a')
```




    97




```python
ord("A")
```




    65



### Methods in strings
Here we have in built strings in python, these are the tools and each string has a new memory location.


```python
x='pyhton'
print(x, type(x))
dir(x)
```

    pyhton <class 'str'>
    




    ['__add__',
     '__class__',
     '__contains__',
     '__delattr__',
     '__dir__',
     '__doc__',
     '__eq__',
     '__format__',
     '__ge__',
     '__getattribute__',
     '__getitem__',
     '__getnewargs__',
     '__getstate__',
     '__gt__',
     '__hash__',
     '__init__',
     '__init_subclass__',
     '__iter__',
     '__le__',
     '__len__',
     '__lt__',
     '__mod__',
     '__mul__',
     '__ne__',
     '__new__',
     '__reduce__',
     '__reduce_ex__',
     '__repr__',
     '__rmod__',
     '__rmul__',
     '__setattr__',
     '__sizeof__',
     '__str__',
     '__subclasshook__',
     'capitalize',
     'casefold',
     'center',
     'count',
     'encode',
     'endswith',
     'expandtabs',
     'find',
     'format',
     'format_map',
     'index',
     'isalnum',
     'isalpha',
     'isascii',
     'isdecimal',
     'isdigit',
     'isidentifier',
     'islower',
     'isnumeric',
     'isprintable',
     'isspace',
     'istitle',
     'isupper',
     'join',
     'ljust',
     'lower',
     'lstrip',
     'maketrans',
     'partition',
     'removeprefix',
     'removesuffix',
     'replace',
     'rfind',
     'rindex',
     'rjust',
     'rpartition',
     'rsplit',
     'rstrip',
     'split',
     'splitlines',
     'startswith',
     'strip',
     'swapcase',
     'title',
     'translate',
     'upper',
     'zfill']




```python
print(dir(x))
```

    ['__add__', '__class__', '__contains__', '__delattr__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__getitem__', '__getnewargs__', '__getstate__', '__gt__', '__hash__', '__init__', '__init_subclass__', '__iter__', '__le__', '__len__', '__lt__', '__mod__', '__mul__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__rmod__', '__rmul__', '__setattr__', '__sizeof__', '__str__', '__subclasshook__', 'capitalize', 'casefold', 'center', 'count', 'encode', 'endswith', 'expandtabs', 'find', 'format', 'format_map', 'index', 'isalnum', 'isalpha', 'isascii', 'isdecimal', 'isdigit', 'isidentifier', 'islower', 'isnumeric', 'isprintable', 'isspace', 'istitle', 'isupper', 'join', 'ljust', 'lower', 'lstrip', 'maketrans', 'partition', 'removeprefix', 'removesuffix', 'replace', 'rfind', 'rindex', 'rjust', 'rpartition', 'rsplit', 'rstrip', 'split', 'splitlines', 'startswith', 'strip', 'swapcase', 'title', 'translate', 'upper', 'zfill']
    


```python
x.upper()
```




    'PYHTON'




```python
x = 'PYTHON'
print(x)
x.lower()
```

    PYTHON
    




    'python'




```python
def foo(x):
    s = ''
    for ele in x:
        if ord(ele) in range(65, 95):
            s+=chr(ord(ele)+32)
        else:
            s+=ele
        return s
```

### Toung twister


```python
tt ='''peter piper picked a peak of pickled peppers.
peck of pickled peppers iper picked.
peter piper picked a peak of pickled peppers,
where's the peak of pickled peppers peter piper picked
'''
tt
```




    "peter piper picked a peak of pickled peppers.\npeck of pickled peppers iper picked.\npeter piper picked a peak of pickled peppers,\nwhere's the peak of pickled peppers peter piper picked\n"




```python
x = [1, 2, 3]
id(x)
```




    1800210180288



strings are <u>**'immutable'**</u>, the resulting strings from string methods have a newmember location
in order to use these strings, we need reassign

### Lowercase function
In pyhton the lower() function will covert the whole characters into lower() function form like (a,b,c,d,....).


```python
a ='''peter piper picked a peak of pickled peppers.
peck of pickled peppers iper picked.
peter piper picked a peak of pickled peppers,
where's the peak of pickled peppers peter piper picked
'''
a.lower()
```




    "peter piper picked a peak of pickled peppers.\npeck of pickled peppers iper picked.\npeter piper picked a peak of pickled peppers,\nwhere's the peak of pickled peppers peter piper picked\n"



### Uppercase function
In pyhton the upper() function will covert the whole characters into upper() function form like (A,B,C,D,....).


```python
### upper
a.upper()
```




    "PETER PIPER PICKED A PEAK OF PICKLED PEPPERS.\nPECK OF PICKLED PEPPERS IPER PICKED.\nPETER PIPER PICKED A PEAK OF PICKLED PEPPERS,\nWHERE'S THE PEAK OF PICKLED PEPPERS PETER PIPER PICKED\n"



### Capitalize
In pyhton capitalize() willconvert the first character into capital letter and the remaining characters will be in lower case.


```python
a.capitalize()
```




    "Peter piper picked a peak of pickled peppers.\npeck of pickled peppers iper picked.\npeter piper picked a peak of pickled peppers,\nwhere's the peak of pickled peppers peter piper picked\n"



### Title
The title function will convert the given input of a every string of first character into the uppercase form.


```python
### title : converts 1st alphabet of every word in the string
a.title()
```




    "Peter Piper Picked A Peak Of Pickled Peppers.\nPeck Of Pickled Peppers Iper Picked.\nPeter Piper Picked A Peak Of Pickled Peppers,\nWhere'S The Peak Of Pickled Peppers Peter Piper Picked\n"



### Split
The split() function means it will give the each and every string into the new line.


```python
### split
a.split()
```




    ['peter',
     'piper',
     'picked',
     'a',
     'peak',
     'of',
     'pickled',
     'peppers.',
     'peck',
     'of',
     'pickled',
     'peppers',
     'iper',
     'picked.',
     'peter',
     'piper',
     'picked',
     'a',
     'peak',
     'of',
     'pickled',
     'peppers,',
     "where's",
     'the',
     'peak',
     'of',
     'pickled',
     'peppers',
     'peter',
     'piper',
     'picked']



###  Swapcase
The swapcase can change the input that you have given into  [upper() to lower()]  (or)  [lower() to upper()] characters that are given by capital letter will transform into normal letters, normal letters will transfrom into capital letter.


```python
a.swapcase()
```




    "PETER PIPER PICKED A PEAK OF PICKLED PEPPERS.\nPECK OF PICKLED PEPPERS IPER PICKED.\nPETER PIPER PICKED A PEAK OF PICKLED PEPPERS,\nWHERE'S THE PEAK OF PICKLED PEPPERS PETER PIPER PICKED\n"




```python
b = "We have joined the DATA ANALYTICS"
b.swapcase()
```




    'wE HAVE JOINED THE data analytics'



### Casefold function
 The casefold() changes string lower case to more lowercase, special character like germen character (ß) is already in lower case so, the lower method doesn’t make the conversion.
 
 The casefold() method will convert ß to its equivalent character ss.


```python
x = 'ß'
x.casefold()
```




    'ss'



## 2).Explain why strings are Immutable by taking a string method as an example. 

The strings are immutable because the each string has separate memory locations


```python
x = 'siddu'
x.upper()
```




    'SIDDU'




```python
print(id(x), id(x.upper))
```

    1937139417008 1937147288752
    

Here the identity values are different means the memory locations are different, so the string are immutable.

### 3). Take a two strings of your choice, 
#### i).Reverse one string
#### ii).Concatenate these two strings
#### iii).Get the alternate chars of the concatenate string in reverse order.


##### i). Reverse one string
it begins with index -1 to -n , where n is length of string
    
 negitive indexing moves from right to left.


```python
x = 'hyderabad'
y = 'charminar'
z = y[::-1]
print(x + z)
```

    hyderabadranimrahc
    

#####  ii). Concatenate these two strings
string concatenation is the operation of joining character strings end-to-end.



```python
str1="hyderabad"
str2="charminar"
print ("String 1:",str1)
print ("String 2:",str2)
str=str1+str2
print("Concatenated two different strings:",str)
```

    String 1: hyderabad
    String 2: charminar
    Concatenated two different strings: hyderabadcharminar
    

#####  iii). Get the alternate chars of the concatenate string in reverse order.
 Here we take two strings then we add these two strings by using concatination.
 
 After concatination the output will be taken for another function called reverse() function.


```python
x = 'hyderabad'
y = 'charminar'
z = x + y
print(z)
print(z[::-2])
```

    hyderabadcharminar
    rnmacaaey
    
