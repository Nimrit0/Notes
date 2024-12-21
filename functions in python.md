
functions provides reuseability.

```python
def add_two(a,b):
	return a+b
total = add_two(5,4)
print(total)

print(add_two(6,7))
```

function return or print your choice!

function inside function 

```python
#function inside a function

  
  

# 7 6 5    7+6 = 14 +5 18?

  

def ad_first(num1,num2):

    return num1+num2

  
  

def ad_second(num1,num2):

    return num1+num2

  

#we wil be dealing with three numbers adding them

  

def total_add(num1,num2,num3):

    sub = ad_first(num1,num2) #function inside another function

    total = ad_second(num3,sub)

    print(total)

  

total_add(7,6,5)```


kiss : keep it simple stupid.


default argument


```python
def details(firstname,lastname,age=20):

    print(firstname)

    print("\n")

    print(lastname)

    print("\n")

    print(age)

  

details("nirmit","baskota") # here the age is default parameter
```


variable scope

```python
x =5 # global variable

def fun()
	x =7 #local variable
	return x
print(fun())
print(x)

# global x : to create a local variable a global varaible.

```

## list in python

data structure 

ordered collection of item 

you can store anything in lists int,float,string or even mixed data!!



```python

number = [1,2,3,4,5]
print(numbers)
words = ["apple","banana","grapes"]

mixed = [1,2,3,4,"five","six","seven",3.2,4.2,None]
print(mixed)

#you can use the slicing to print

print(mixed[0:4])

# To update data of lists

mixed[1] = 0 # here the value 2 will be replaced by 0

print(mixed)


```


how to add items to our list
most commoon thing that you can do with your list and most imortant

<span style="color:rgb(0, 176, 240)">append method : adds data in last index</span>

```python
fruits = ["grapes","apple","baanana"]
print(fruits)

fruits.append('mango')

# we use append in real world life like

vegetables =[]

vegetables.append("onion")
vegetables.append("tomato")
vegetables.append("potato")

print(vegetables)


```


<span style="color:rgb(0, 176, 240)">insert method: adds data to list according to the indexing</span> 


```python

fruits1 = ["mango","orange"]
fruits1.insert(1,"grapes")
print(fruits1)

```


combining two list or concatinating two lists

```python
fruits1 = ["apple","mango"]
fruits2=["banana","pineapple"]
fruits = fruits1 + fruits2

print(fruits1)
print(fruits2)
print(fruits)

#extend method

fruits1.extend(fruits2)
print(fruits1)

#append method

fruits1.append(fruits2) #list inside list

```


DELETE methods in list


pop method 
del fruits[1]
fruits.remove('banana') : when you know the name of list item instead of indexing.if we have two bananas then it will only remove first banana.

```python
fruits = ["apple","orange","banana"]
fruits.pop()#by default it will delete the first option if you don't set an argument 
print(fruits)

fruits.pop(1)
del fruits[1]

print(fruits)

```


in keyword with list


```python
fruits = ["orange","apple","mango"]

if 'apple' in fruits:
	print("apple is presentt")
else:
	print("apple is not present")
	
```


some more list methods in list

```r

#count : to count how many times it's repeated
#sort method :alphabetically
#sorted fuction : just sort them doesn't change the orginal value
#clear method: it empties or list
#copy method : copies the list
#rewverse method: it reverses the list

fruits =["orange","apple","pear","bananna","apple"]
print(fruits.count("apple"))

fruits_copy = fruits.copy()
print(fruits_copy)

To sort in descending order, we could use numbers.sort(reverse=True)
```


IS VS EQUAL  list comparision

== , is 

```
fruits1 = ['orange','apple','pear']
fruits = ['orange', 'apple','pear']

print(fruits1==fruits2) //values are same

print(fruits is fruits2)//false because both are in different location although the value is same
```


split method

```r
convert string to list

user_info = "nirmit baskota 22 hacker".split()

user_info1 = "nirmit,baskota,22,hacker".split(',')


#join method

user_info3 =['harshit','24','develper']
a = ','.join(user_info3)


```

list vs array

array: orderd collection of item
list : store any data /flexible

c , c++ , java

only store one data type

python

can store any data type

python module : fix data type 

javascript array = python list


### list vs string

strings are immutable which means you cannot change them 

lists are mutable which means you cannot change them

for example

```r
s = "string"
t = s.title()
print(t)# here the title method is not changing the orginal value of s

l = ['word','word2','word3']
l.pop()
print(l) #here the l is mutable 
```

 
looping in list


```r
fruits = ['apple','banana','orange','pear']
for fruit in fruits:
	print(fruit)
```

we don't use while loop in list but we can also use it

```
fruits = ['apple','banana','orange','pear]
i =0
while i<len(fruits):
	print(fruits[i])
```

list inside list


```r
matrix =[[1,2,3],[4,5,6],[7,8,9]]#also known as 2d list
#there are 3 items

print(matrix[0])

#to print all items

for i in matrix:
	for j in i:
		print(i)

print(matrix[1][3])

```


type function : it is use to check the data type of any variable


s = "string"

print(type(s))




## more about list

generating list using range function

```r
numbers = list(range(1,11))
print(numbers)
```


something more abou pop method

```r
number = list(range(1,11))
number.pop()
print(numbers)

#pop method also return the value
```



index method is also used in list to find the item in the list for eg:

```r
number = list(range(1,11))
print(number.index(1,3,14)) #here the searching is starting from 3 rd position  and the 14 means where to stop the searching

```


passing list into function

```r
numbers = list(range(1,22))
print(numbers)

def negative_list(l):
	negative = []
	for i in l:
		negative.append(-i)
	return negative
print(negative_list(numbers))
```




## min and max


numbers = [50,34,24]

print(min(numbers))
print(max(numbers))



