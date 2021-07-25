## Build A Random Name Generator Using Python

How many times have you found yourself trying to figure out which name you should use because you would not want to publicly use you name in website or app registration? If it's many then you surely should try building an app that can randomly give you different names to use when in need.

This app is written in python,
# What you will need
* A code Editor (**preferred pycharm**)
* A environment
and you will be good to go  

first you will have to import two packages:

``` python
import requests
from random import randint
```
next you will need a url with different names in it 

``` python
url = 'https://svnweb.freebsd.org/csrg/share/dict/propernames?revision=61766&view=co'
```
using the requests you have to fetch the data from url and and convert it to text  run the print to confirm all names display in terminal

``` python
r = requests.get(url)
text = r.text
print(text)
```
the names will display in different line, use the split library to clear the blank spaces and print to confirm, you can spot the difference

``` python
individual_word = text.split()
print(individual_word)
```
To make it randomly generate names you will have to use the randint, now and print to see randomly generated word:

``` python
random_number = randint(0, len(individual_word))
print(individual_word[random_number])
```
### Get the whole code [Here](https://github.com/larymak/Python-project-Scripts/tree/main/RandomNameGen)

## Enjoy Coding
## Follow me  
[Twitter](https://twitter.com/larymak1)  
[GitHub](https://github.com/larymak)  
[YouTube](https://www.youtube.com/channel/UCrT1ARRZfLOuf6nc_97eXEg)  
[More Blog](https://larymak.hashnode.dev/)  