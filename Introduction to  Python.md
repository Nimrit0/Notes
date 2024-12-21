 
```python
print("hello world")
print('hello world')
print('''hello world''')
```

string -> collection of character inside "double quotes" or 'single quotes'

You can use 'single quote ' inside "double quotes"

or 

"Double quotes " inside 'single quotes'

example

```python
print("hello 'world' ")
print('hello "world"')
```


Note: cannot use single quote inside single quote and vice versa

``` python
print('hello 'world' ')
```


## Escape sequences

```python
print("hello \"world\" how are you")
print('i am fine \'btw\' how are you ')
```


| Escape Sequences | Meaning   of the sequences |
| ---------------- | -------------------------- |
| \\'              | single quote               |
| \\"              | double quote               |
| \\\\             | backslash                  |
| \\n              | new line                   |
| \\t              | tab                        |
| \b               | backspace                  |


## comments

comments are basically use by developer to understand the code


```
#single line comment

```


Escape character as  normal text

suppose you want this as output

```
output : Line A \n Line B
```


## printing emojis 

you need the unicode of the emojis 


https://unicode.org/emoji/charts/full-emoji-list.html

```r
U+1F600
```

in program replacing '+' with 3 zeroes

```r
print("\U0001F600')
```


## python as a calculator

```
print(2*3+4)
```




| Operators in py | Description of the operators | Suitable example |
| --------------- | ---------------------------- | ---------------- |
| +               | Addition                     | print(2+3)       |
|                 |                              | 5                |
| -               | Subtraction                  | print(2-3)       |
|                 |                              | -1               |
| *               | multiplication               | print(2*3)       |
|                 |                              | 6                |
| /               | float division               | print(4/2)       |
|                 |                              | 2.0              |
| //              | integer division             | print(2*4)       |
|                 |                              | 8                |
| %               | modulo,it gives remainder    | print(5%2)       |
|                 |                              | 1                |
| **              | exponent                     | print(2**3)      |
|                 |                              | 8                |
|                 |                              |                  |


```r
print(2**0.5)
print(round(2**0.5,4))
```

Precedence rule

To evaluate complex expression python follows the rule of precedence, it governs the order in which the operation take place.


```r
print(2+5*2)
```


| Operators used in python | precedence and Associativity Rule |
| ------------------------ | --------------------------------- |
| PARENTHESE               | HIGHEST                           |
| Exponent                 | Right to left                     |
| *,//,/,%                 | Left to Right                     |
| *,-                      | Left to right                     |
|                          |                                   |
|                          |                                   |


rules and conventional in python

conventional means like a recomendation

for eg:

```python
user_name = "Rohit"  #snake case writing used in python
userName = "mohit" # camel case writing used in java

```

## string

strings is a collection of character inside single quotes or double quotes.

```python
first_name = "Nirmit"
last_name = "baskota"
full_name = first_name + " " + last_name
print(full_name)
print(first_name + "3")
print(first_name + str(3))
```


```python
first_name = "Nirmit"  
last_name = "baskota"  
study= "bachleor"  
age = 20  
print("my name is " + first_name + " " + last_name +" " + "i am " +str(age)+" " + "i read in" + " "+study)
```


## input function 

Note : input functiojn by default takes input in string 

input function 

```python
name = input("enter your name ")
print("hello" + name)
age = input("what is your age? ")
print("your age is "+ age)
```

```python
first_number = int(input('enter first name '))
second_number = int(input("enter second number ))
print(first_number + second_number)
```


## more about variable 

This type of variable assignment in Python is called **multiple assignment** or **tuple unpacking**. It allows you to assign values to multiple variables in a single line. In your example:

```python
name, rollno, sec = "nirmit", "24", 'A'
```

```python
x = y = 1
```


## single line input two variable

```python
name , age = input("Enter your name and age separated by : ok ?  ").split(":")
print(name)
print(age)
print(type(name))
print(type(age))
```


## string formatting

```python
name = "nirmit"
age = 24
print("hello" + name + " "+ "your age is " +str(age)) #ugly code
```

in python 3 !

```python
print("hello {} your age is {}.format(name,age)) #used in python3

print(f"hello {name} your age is {age +2}) #used in upper python 3.6
```


## string indexing in python

```python
language = "python"

#postion (index number)

# p = 0     or from 6th last -6
# y = 1     or from 5th last -5
# t = 2     or from 4th last -4 
# h = 3     or from 3rd last -3
# o = 4     or from second last -2 
# n = 5     or from last  -1

print(language[4])
```

### string slicing in sub sequence

```python
lang = "python"

#syntax --> start argument :  stop argument - 1 : step argument not mandatory


print(lang[0:-1])

print(lang[0:5:2])
```

## string methods in python

```python
name = "Nirmit Baskota"

# 1 len () function

print(len(name)) # it also counts the space

# use use dots in method
# 2 lower() method

print(name.lower())

# 3) upper() method

print(name.upper()) 

# 4) title method

#  5) strip method  : it is use to remove the spaces rstrip() removes right spaces and lstrip removes the left strip


# 6) replace method : it is use to replace character or string

# 7) find method : it is used to find the position of character or string

#8 center method : it is used to add something (character) either infront or backward of a string.

nam = "nirmit"
print(nam.center(11,"*"))







a = "nirmit baskota is a good boy"

print(a.replace("is","was"))

print(a.find("is",1)) # 1 indicates start from the 1st position


a = "      nirmit      baskota       "

print(name.title()) #it capilatilzed the first character of the passed string

#5 count() method # it counts that a char is repeated how many times

print(name.count("a"))
print(a.strip())

```


```python
name = input("Enter a sentences : ")  
  
print(f"The number of words in the sentence is {(name.count(" "))+1}")
```

### string is immutable means non changeble


```python
string = "string"
string.replace('t','T')
print(string) # here the string is not changed

#instead you can use this

name = "nirm"
name = name +"it
print(name)


```

in ruby  string is muttable!


## condition operator


```python
a = int(input("Enter your age " ))
if(a>18):
	print("you are allowed to play games")
else:
	print("you are not allowed to play games)
```


```python
x = 18
if x>18:
	pass
```

```python
if elif else
or and 
nested if

```

```python
#in keyword in python

name = "nirmit baskota"
if 'a' in name:
	print("a is present")
else:
	print("a is not present")
```

```python

#check empty or not

name = "nirmit"
if name:
	print("not empty true")
else:
	print("empty false")

```


## loops in python

while loop syntax

```python
i =1
while i<=10:
	print("hello world")
	i = i +1
```

infinite loops in python

```python
#infinite loop
i =0
while i<=10:
	print("hello world")



#boolean in python true or false


while True:
	print("always true" )
```


for loop in python with range function

 ```python
 for i in range(10):# 0 to 10
	 print(f"hello world : {i}")


for i in range(1,11) # it will iterate upto 10 but will not include 11

#you can also add step arguments

for in rangae(1,11,2) # step arugument used for printing even number


for i in range(10,-1,-1)


```

break  and continue keyword

```python
#break : it will terminate the whole programm after getting 5
for i in range(1,11):
	if i==5:
		break
	print(i)



#continue it will skipp the 5

for  i in range(1,11):
	if i==5:
		continue
	print(i)
```

DRY principle of coding: don't repeat yourself



```python
#works in every programming language
name = "nirmit"
for i in range(len(name)):
	print(name[i])


#works only in python
name = "baskota"

for i in name:
	print(i)
```




