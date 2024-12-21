
## tuple

tupld is also like list like data structure
tuple can store any data type
most important tuples are immutable , once tumple is created you can't update 
data inside tuple

no append , no insert ,no pop, no remove

when we don't have any changes in data we use tuple and it's faster than list


tuples method

count
index --> to find the postion of any character
len function -->
slcing

```r
example = ('one','two','three')
print(example[1:3])
```




looping in tuples

```r
mixed = (1,2,3)
for i in mixed:
	print(i)
```


tuple with one element

```r
nums = (1)
words = ('word1') 

///both of them are not tuple

nums = (1,)
words = ('words',)
print(type(nums))

```


tuple without parenthesis

```r
guitars = 'yahoo','baton rouge','taylor'

print(type(guitars))

```


tuple unpacking 

```r
guitarists = ('manali jamal','eddie van der meer','haha','lol')

guitarist1,guitarist2,guitarlist3 =(guitarists)

```

list inside tuple

```r
favorites = ('southern mangolia',['tokyo ghoul theme', 'landscape'])

favorites[1].append("we made it")

```


function in tuple

```
min () max() sum
```


function returning two values it's in tuple form so we need to unpack it for example

```r
def func(int1,int2):
	add = int1+int2
	multiply = int1 * int2
	reutrn add,multiply

print(func(5,6)) //it wil return tuple

//let's unpack it

add, multiply = fun(4,5)
print(add)
print(multiply)
```

something more about tuples , list, str

```r
nums = tuple(range(1,11))
print(nums)

#converting tuple into list

haha = str(tuple(range(1,1)))


```



## dictionaries intro

because of limitation of lists, lists are not enough to represent real data.

unorderd collections of data in key : value pair.

//how to create a dictioinaries


```r
user = {'name' : 'Harshit','age':24 }
print(type(user))

or

user1 = dict(name ="harshit",age=24)
print(type(user1))
```

no indexing in dictionaries

to access the data we use the key

```r
user = {'name' : 'nirmit','age':24}
print(user['age'])
```

//how to add data to empty dictionary

```r
user_info2 = {}

user_info2['name']='mohit'
print(user_info2)
```


///in keyword and iteration in dictinoary


```r
user_info = {
	'name': 'nirmit',
	'age' : 24,
	'roll' : 14',
	'sec' : 'A',
	
}

//check if key exist or not
if 'name' in user_info:
	print("it's present")

//check if value exist or not

if 'nirmit' in user_info.values(): //we will use values method 
print("its present")
```

## loops in dictinoary

```r
user_info = {
	'name' : 'nirmit',
	'age' : '53',
	'roll' : 14,
	
}

for i in user_info:
	print(i)#display only keys

#for values

for in in user_info.values():
	print(i)

#values method

user_info_values = user_info.values()
print(user_info_values)



#keys method

user_info_keys = user_info.keys()
print(user_info_keys)


#items method

user_items = user_info.items()
print(user_items)
print(type(user_items))
# it returns typle list
#[('name','nirmit'),('age','20')]

for key, value in user_info.items():
	print(f"key is {key} and value is {value})
```


## dictionary data add data delete


```
#add and delete data

user_info = {
	'name' : 'harshit',
	'age' : 24,
	'fav_movies' : ['coco','kimi', 'no']
}

#how to add data

user_info['fav_songs']=['songs','songs2']

#pop method

user_info.pop('fav_movies')#return the deleted values





```





