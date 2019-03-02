Python Cheatsheet
=================

<sup>[Fork this on GitHub](https://github.com/BisratYalew/python-cheatsheet)
</sup>


## About
I have created this cheatsheet with intention of collecting python code snippets that I used on my projects/programs and from the internet for reducing coding hours and making other developers life easier.




String
------


```python
>>> check = '    Python is great!     '  # removes characters from both left and right based on the argument
>>> check.strip()
'Python is great'
>>> check.lstrip()
'Python is great!     ' ## removes characters from left based on the argument
>>> check.rstrip() ## removes characters from left based on the argument
'     Python is great!'
```



### ord()
```python
>>> ord('A'), ord('Z')
(65, 90)
>>> ord('0'), ord('9')
(48, 57)
>>> ord('a'), ord('z')
(97, 122)
>>> ord('B'), ord('Y')
(66, 89)
```


#### The in and not in Operators with string
```python 
>>> 'Python' in 'Python is great!'
True
>>> 'python' in 'Python'
True
>>> 'PYTHON' in 'Python is great!'
False
>>> '' in 'python'
True
>>> 'Python' not in 'python and javascript' ## Matches case
False
```

#### The in and not in Operators with list
```python 
>>> a = ['P', 'y', 't', 'h', 'o', 'n']
>>> 'p' in a
False
>>> 'P' in a
True
>>> 'o' in a
True

## On Integers List
>>> a = [1, 2, 3, 5]
>>> 5 in a
True
>>> 4 in a
False
>>> 1 in a
True
```


### The upper(), lower(), isupper(), islower() string methods

```python
>>> check = 'Hello world!'
>>> check = check.lower() ## converts check to lower
>>> check
'hello world!'
>>> check = check.isupper() ## checks whether check variable is upper or not. 
False
>>> check = check.islower() ## checks whether check variable is upper or not. 
True
>>> check = check.upper() ## converts check to upper
>>> check
'HELLO WORLD!'
>>> check = check.isupper() ## checks whether check variable is upper or not. 
True
>>> check = check.islower() ## checks whether check variable is upper or not. 
False
```


### Template Strings
##### <i>Template strings are a simpler mechanism which are used to handle format strings generated by users</i>

```python
>>> from string import Template
>>> language = 'Python'
>>> t = Template('$name is great!')
>>> t.substitute(name=language) ## Substitutes name with language variable
'Python is great!'
```

### Pyperclip module
##### <i>Pyperclip is python library that help us easily copy and paste string</i>

##### First Install it using pip

```
pip install pyperclip
```

```python
>>> import pyperclip
>>> pyperclip.copy('Hello World') ## Copy Hello World
>>> pyperclip.paste()
'Hello World'
```


## Contributing

Feel free to contribute and send pull requests

## Author

* [BisratYalew](https://bisratyalew.github.io)

