# <i><u> BASIC TERMINOLOGIES :</i></u>
### STRING :
A string is a sequence of characters. For example, "hello" is a string containing a sequence of characters 'h' , 'e' , 'l' , 'l' , & 'o'.
* A string is a sequence of one or more characters (letters, numbers, symbols) that can be either a constant or a variable. Made up of Unicode, strings are immutable sequences, meaning they are unchanging.
### CLASS :
A class is a user-defined data type that contains both the data itself and the methods that may be used to manipulate it.Classes serve as a template to create objects.
* A class describes the contents of the objects that belong to it: it describes an aggregate of data fields (called instance variables), and defines the operations (called methods).
##### SYNTAX : Syntax: Object Definition. obj = ClassName() print(obj.atrr) 
### OBJECT :
 Objects are the instances of a particular class. 
* EXAMPLE :Suppose Bike is a class then we can create objects like bike1 , bike2 , etc from the class.
### METHOD :
 Methods are functions that are associated with an object and can manipulate its data or perform actions on it.
* In a Python class, we can define three types of methods:
1. Instance methods.
2. Class methods.
3. Static methods.
### PARAMETER :
* A parameter is the variable listed inside the parentheses in the function definition.
* Parameter should be within the parentheses of the function.
### ASCII :
* ASCII stands for American Standard Code for Information Interchange. It is a numeric value given to different characters and symbols, for computers to store and manipulate. For example, the ASCII value of the letter 'A' is 65.
### DIRECTORY :
* The dir() function returns all properties and methods of the specified object, without the values.
* This function will return all the properties and methods, even built-in properties which are default for all object.

# <u><i> STRING METHODS: </i></u> 


```python
a = "string" 
dir(a) # ALL THE METHODS PRESENT IN CLASS
```




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



### 1. ord(): [order]
* The ord() function returns the number representing the unicode code of a specified character.
* ord(ch) returns the byte value for a character - "a" is 65, "b" is 66, etc.  


```python
#EXAMPLE :
ord('A') # HERE NO. REPRESENTING THE UNICODE OF THE CHARACTER 'A' IS GIVEN AS OUTPUT
```




    65




```python
ord('a') # SIMILARLY HERE NO. REPRESENTING THE UNICODE OF THE CHARACTER 'a' IS GIVEN AS OUTPUT
```




    97



## 2. lower() : [lowercase]


```python
str1 = "You must be the change you wish to see in the world."
str1.lower() #COMPLETE STRING IS DISPLAYED IN LOWERCASE LETTERS
```




    'you must be the change you wish to see in the world.'



## 3. upper() :[uppercase]
*  The upper() method returns the uppercased string from the given string.


```python
str1.upper() #COMPLETE STRING IS DISPLAYED IN UPPERCASE LETTERS
```




    'YOU MUST BE THE CHANGE YOU WISH TO SEE IN THE WORLD.'



## 4. capitalize() :
* 1st alphabet of the string is capital.


```python
str1.capitalize() #1ST ALPHABET IN THE COMPLETE STRING IS CAPITAL"
```




    'You must be the change you wish to see in the world.'



## 5. title() :
* This method changes first alphabet of every word will convert into capital letter


```python
str1.title() #FIRST ALPHABET OF EVERY WORD IN THE STRING IS CAPITAL
```




    'You Must Be The Change You Wish To See In The World.'



## 6. swapcase() :
* This method changes capital letters to small letters and small letters to capital letters


```python
swap = "Hare Krishna"
swap.swapcase() #IT PRINTS LOWERCASE TO UPPERCASE LETTERS, UPPERCASE TO LOWERCASE LETTERS
```




    'hARE kRISHNA'



## 7. casefold() :

* This method changes string lower case to more lower case , special characters like Germen character (ß) is already in lower case so, the lower method doesn’t make the conversion.
* The casefold() method will convert ß to its equivalent character ss



```python
B = 'German ss is ß'
B.casefold()
```




    'german ss is ss'



## 8. help():
*  If no argument is given, the interactive help system starts on the interpreter console. If you want to get out of help console, type quit.
* We can also get the help documentation directly from the python console by passing a parameter to help() function.
* Syntax : help(object)



```python
help(object) # IT INVOKES BUILT IN HELP SYSTEM
```

    Help on class object in module builtins:
    
    class object
     |  The base class of the class hierarchy.
     |  
     |  When called, it accepts no arguments and returns a new featureless
     |  instance that has no instance attributes and cannot be given any.
     |  
     |  Built-in subclasses:
     |      anext_awaitable
     |      async_generator
     |      async_generator_asend
     |      async_generator_athrow
     |      ... and 93 other subclasses
     |  
     |  Methods defined here:
     |  
     |  __delattr__(self, name, /)
     |      Implement delattr(self, name).
     |  
     |  __dir__(self, /)
     |      Default dir() implementation.
     |  
     |  __eq__(self, value, /)
     |      Return self==value.
     |  
     |  __format__(self, format_spec, /)
     |      Default object formatter.
     |  
     |  __ge__(self, value, /)
     |      Return self>=value.
     |  
     |  __getattribute__(self, name, /)
     |      Return getattr(self, name).
     |  
     |  __getstate__(self, /)
     |      Helper for pickle.
     |  
     |  __gt__(self, value, /)
     |      Return self>value.
     |  
     |  __hash__(self, /)
     |      Return hash(self).
     |  
     |  __init__(self, /, *args, **kwargs)
     |      Initialize self.  See help(type(self)) for accurate signature.
     |  
     |  __le__(self, value, /)
     |      Return self<=value.
     |  
     |  __lt__(self, value, /)
     |      Return self<value.
     |  
     |  __ne__(self, value, /)
     |      Return self!=value.
     |  
     |  __reduce__(self, /)
     |      Helper for pickle.
     |  
     |  __reduce_ex__(self, protocol, /)
     |      Helper for pickle.
     |  
     |  __repr__(self, /)
     |      Return repr(self).
     |  
     |  __setattr__(self, name, value, /)
     |      Implement setattr(self, name, value).
     |  
     |  __sizeof__(self, /)
     |      Size of object in memory, in bytes.
     |  
     |  __str__(self, /)
     |      Return str(self).
     |  
     |  ----------------------------------------------------------------------
     |  Class methods defined here:
     |  
     |  __init_subclass__(...) from builtins.type
     |      This method is called when a class is subclassed.
     |      
     |      The default implementation does nothing. It may be
     |      overridden to extend subclasses.
     |  
     |  __subclasshook__(...) from builtins.type
     |      Abstract classes can override this to customize issubclass().
     |      
     |      This is invoked early on by abc.ABCMeta.__subclasscheck__().
     |      It should return True, False or NotImplemented.  If it returns
     |      NotImplemented, the normal algorithm is used.  Otherwise, it
     |      overrides the normal algorithm (and the outcome is cached).
     |  
     |  ----------------------------------------------------------------------
     |  Static methods defined here:
     |  
     |  __new__(*args, **kwargs) from builtins.type
     |      Create and return a new object.  See help(type) for accurate signature.
     |  
     |  ----------------------------------------------------------------------
     |  Data and other attributes defined here:
     |  
     |  __class__ = <class 'type'>
     |      type(object) -> the object's type
     |      type(name, bases, dict, **kwds) -> a new type
    
    

## 9. find(): 
* find() method returns the lowest index or first occurrence of the substring if it is found in a given string.
    If it is not found, then it returns -1.

* Syntax: str_obj.find(sub, start, end)
##### Parameters:

* sub: Substring that needs to be searched in the given string.
* start (optional): Starting position where the substring needs to be checked within the string.
* end (optional): End position is the index of the last value for the specified range. It is excluded while checking.





```python
print(str1)
```

    You must be the change you wish to see in the world.
    


```python
str1.find('e') # THE INDEX VALUE OF 1ST SUBSTRING "e" IS 10.
```




    10




```python
str1.find('u',3) #THE INDEX VALUE OF 1ST SUBSTRING "u" IS 5.
#SINCE START POSITION IS "3" IT IS GOING TO CHECK SUBSTRING FROM START POSITION.
```




    5




```python
str1.find('o',20,50) #THE INDEX VALUE OF 1ST SUBSTRING "o" IS 24. SINCE START IS 20, THE SUBSTRING "o" IS CHECKED FROM START STRING
```




    24




```python
help(str1.find)
```

    Help on built-in function find:
    
    find(...) method of builtins.str instance
        S.find(sub[, start[, end]]) -> int
        
        Return the lowest index in S where substring sub is found,
        such that sub is contained within S[start:end].  Optional
        arguments start and end are interpreted as in slice notation.
        
        Return -1 on failure.
    
    

## 10. rfind():

* rfind() method returns the rightmost index of the substring if found in the given string.
* If not found then it returns -1.

* Syntax: str.rfind(sub, start, end)
#### Parameters:

* sub: It’s the substring that needs to be searched in the given string.
* start: Starting position where the sub needs to be checked within the string.
* end: Ending position where suffix needs to be checked within the string.



```python
help(str1.rfind)
```

    Help on built-in function rfind:
    
    rfind(...) method of builtins.str instance
        S.rfind(sub[, start[, end]]) -> int
        
        Return the highest index in S where substring sub is found,
        such that sub is contained within S[start:end].  Optional
        arguments start and end are interpreted as in slice notation.
        
        Return -1 on failure.
    
    


```python
name = "gajularamaram"
name
```




    'gajularamaram'




```python
name.rfind('a') # IT CHECKS FROM BACK AND FINDS THE SUBSTRING POSITION &GIVES POSITVE INDEXING FROM( L -> R)
```




    11




```python
name.rfind('a',2,11)
```




    9



<img src ="attachment:rfind%20.jpg"
     align ="left"
     width ="500">

<img src ="rfind .jpg"
     align = "left"
     width = "500"
     height = "200">


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


```python

```


```python

```
