# Introduction to Python

## Arithmetic operators:
addition: +
subsraction: -
multiplication: *
division: /
exponentiation: **     //2 ** 3 = 8
modulo: %              //find the remainder after dividing   9%2=1
integer division: // round down the division result (only reserve the integer part)   7//2=3  -7//2=-4

## Reserved words in Python:
// False await else import pass None break except in raise True class finally is return and continue for lambda try as def from nonlocal while assert 
del global not with async elif if or yield  

## Some examples given to show the assignment of value in Python (simplified mode):
#The current volume of a water reservoir (in cubic metres)
reservoir_volume = 4.445e8

#The amount of rainfall from a storm (in cubic metres)
rainfall = 5e6

#decrease the rainfall variable by 10% to account for runoff
rainfall *= .9     // equal to rainfall = rainfall * 0.9

#add the rainfall variable to the reservoir_volume variable
reservoir_volume += rainfall

#increase reservoir_volume by 5% to account for stormwater that flows
#into the reservoir in the days following the storm
reservoir_volume *= 1.05

#decrease reservoir_volume by 5% to account for evaporation
reservoir_volume *= 0.95

#subtract 2.5e5 cubic metres from reservoir_volume to account for water
#that's piped to arid regions.
reservoir_volume -= 2.5e5 

#print the new value of the reservoir_volume variable
print(reservoir_volume)

## Boolean 
and: evaluates if both are true 
or: evaluate if at least one ofmany is true
not: flip the bool value
//example: 
age = 14
is_teen = age > 12 and age < 20 
print(is_teen) 
True

//Basic comparison operation
less than: <
greater than: > 
less than or equal to: <=
greater than or equal to: >= 
equal to: ==
not equal to: !=

## Strings 
// examples: 
```
a = 'I wanna quit my PhD' 
print(a)
I wanna quit my PhD 
```
// if there is already quotes in the strings, then back slash is needed, example: 
```
b = "Simon\'s skateboard is in the garage"
print(b)
Simon's skateboard is in the garage
```
// "+" can be used to combine two strings, examlpe: 
```
a = "hello"
b = "world"
print(a+" "+b)
hello world
```
// "*" can be used to repeat the stings, examples:
```
a = "jeremy"
print((a+" ")*5)
jeremy jeremy jeremy jeremy jeremy 
```
// "len" can be used to count the length of a string, example:
```
a="jeremy"
print(len(a))
6
b = "luterbacher"
print(len(a)/len(b))
0.5454545454545454
```
//"[]" can be used to check out the alphabet or number at different locations of the string (always [0] indicates the first one of the string), example:
```
a = 'lebron'
a[0]
'l'
```

## Integer, floats and 
// use type to recognize the types of number, example:
```
type(5.6)
<class 'float'>
```
// type can be changed, example: 
```
a=6.5
int(a)
6
float(a)
6.5
str(a)
'6.5'
```
## string methods: always called with dot 
//"title" can be used to capitalize the name(both first name and last name), example: 
```
#print ("china gao".title()) 
China Gao
```
//several methods can be used and called by ".", examples:
capitalize()      //capitalize() method converts the first character of the string to a capital letter
encode()          //The encode() method returns an encoded version of the string
format()          //Permits you to try and do variable substitutions and data formatting, example:
```
print('Mohanmmed has {} balloons'. format(27))
Mohanmmed has 27 balloons
```
```
a='dog'
b='bite'
print('does your {} {}?'. format(a,b))
does your dog bite?
```

isalpha()         //isalpha() method returns True if all the characters are alphabet letters
islower()         //The islower() method returns True if all characters in the string are lowercase
istitle()         //The istitle() method returns True if all words in a text start with a upper case letter. 
casefold()        //The casefold() method returns a string where all the characters are in lower case
endswith()        //The endswith() method returns True if a string ends with the specified suffix, example:
```
b="abc"
print(b.endswith("c"))
True
```
format_map()      //which is used to return a dictionary key's value, for example:
```
s = 'My name is {name} and I am a {job_title}'
my_dict = {'name': 'Pankaj', 'job_title': 'Software Engineer'}
print(s.format_map(my_dict))
print(s.format(**my_dict))
```
isdecimal()       //The isdecimal() method returns True if all characters in a string are decimal characters, example:
```
s = "28212"
print(s.isdecimal())
True 
```
isnumeric()       //True if all characters in the string are numeric characters.
isupper()         //Check if all the characters in the text are in upper case.
center()          //The center() method will center align the string-----string.center(width[, fillchar])------example:
```
a="jeremy is coming"
print(a.center(24,"*"))
****jeremy is coming****
```
expandtabs()      //The expandtabs() method returns a copy of string with all tab characters '\t' replaced with whitespace characters until the next multiple of tabsize parameter, examlpe:
```
str = 'xyz\t12345\tabc'
print(str.expandtabs())
xyz     12345   abc
```
index()           //The index() method returns the index(location) of a substring inside the string (if found). If the substring is not found, it raises an exception, examlpe:
```
text = 'Python is fun'
print(text. index('s'))
8 (the eighth)
```
isdigit()         // Returns true if all strings are composed of numbers exclusively
isprintable()     // The isprintable() methods returns True if all characters in the string are printable or the string is empty, example:
```
c="/c sees luterbacher" 
print(s. isprintable())
True
```
join()            // Returns a string by joining all the elements of an iterable (list, string, tuple), separated by a string separator, for example:
```
a=['I', 'am', 'Iron', 'man']   // can also be a=('I', 'am', 'Iron', 'man')
print(' '.join(a))             // in this case, use blank to separate words
I am Iron man
```
count()           // The count() method returns the number of occurrences of a substring in the given string, for example:
```
a= "I like chemistry "   
print(a.count('c'))      // can also be: print("the number of c is:",a.count('c')).  // add one more introduction string before the method 
1                        // the output would be: the number of c is: 1                                                       
```
find()            // is used to find the location of a string, for example"
```
a="I will stand on the top of the mountain"
print(a.find('of'))
24
```
// extra conditions can be added to confine the range
```
b= "I will never give up my dream"
print(b. find('i',5,20))         //add conditions in find() brackets, separated by coma. 
14
```
//rfind() can be used to find the last occurance of an index, for example;
```
a='b,c,v,n,n,m'
print(a. rfind('n'))
8
```
isalnum()         // The isalnum() method returns True if all characters in the string are alphanumeric (either alphabets or numbers), for example:
```
name = "M234onica"
print(name.isalnum())
True
```
isidentifier()    // The isidentifier() method returns True if the string is a valid identifier in Python, for example:
```
str = 'Python'
print(str.isidentifier())
True
```
isspace()         // The isspace() method returns True if there are only whitespace characters in the string, for example:
```
s = '   \t'
print(s.isspace())
True
```
ljust().          // The string ljust() method returns a left-justified string of a given minimum width, for example:
```
string = 'cat'
width = 5
print(string.ljust(width))
cat 
```
split().         // breaks up a string **at the specified separator**(the separator should be mentioned in method if there is) and returns a list of strings, for example: 
```
a="lebron is a bullshit"
print(a.split())                    // separate at "blank"
['lebron', 'is', 'a', 'bullshit']
```
```
a="lebron is a bullshit"
print(a.split(","))                 //when the separator is a coma, since there is no coma in string "a", the split would not be processed
['lebron is a bullshit']
```

maxsplit can also be specified to  **choose split from which position**, for example: 
```
grocery = 'Milk, Chicken, Bread, Butter'

# maxsplit: 2
print(grocery.split(', ', 2))

# maxsplit: 1
print(grocery.split(', ', 1))

# maxsplit: 5
print(grocery.split(', ', 5))

# maxsplit: 0
print(grocery.split(', ', 0))
```
output:
```
['Milk', 'Chicken', 'Bread, Butter']
['Milk', 'Chicken, Bread, Butter']
['Milk', 'Chicken', 'Bread', 'Butter']
['Milk, Chicken, Bread, Butter']
```


# Data Structure
## List
// list is the most common and basic data structure **mutable and ordered** in Python, can be created with ***square brackets***, the index starts from zero, for example:
```
list = [1,2,3,4,56,78]
list[0]                //all list starts from index 0 
1
list[3]
4
```
```
b=[3,5,6,6]
len(b)                 //from index 0 to 3, the length of the list is 4. 
4
```
```
a=[2,3,4,5]
a[-1]                  //"-1" is the index of the last one in the list, while "-2" is the second to the last one in the list. 
5
```

//slice a list, for example:
```
months=['january','Feburary','March','April','May','June','July','August','September','October','November','December']
print(months[6:9])     //from index 6 to index 9
['July', 'August', 'September']
print(months[:6])      //print the first half year  
['january', 'Feburary', 'March', 'April', 'May', 'June']
print(months[6:])      //print the second half year
['July', 'August', 'September', 'October', 'November', 'December']
print(months[2:3])     //when slicing, the lower index is inclusive while the upper index is exclusive 
['March']
print(months[::-1])    // "-1" is the interval of slicing, in this case we can list all the elements reversely, [::]can be used to list all range of elements. 
['December', 'November', 'October', 'September', 'August', 'July', 'June', 'May', 'April', 'March', 'Feburary', 'january']
```

// use 'in" or "not in =" to return a bool of whether an ***element exists within the list***, for example:
```
'isa' not in 'american'
True
'isa' in 'china'
False
```

//Mutability: whether or not we can change an object once it has been created. 
```
list= [1,2,3,4]
list[0]='Nick'        //change the list 
print(list)
['Nick', 2, 3, 4]     //a new list is created, so list is mutable.
```
```
a='hellow there'
a[0]
'h'                   // the string starts from index 0   
a[0]='go'
Traceback (most recent call last):    
  File "<stdin>", line 1, in <module>
TypeError: 'str' object does not support item assignment 
```

// Order is whether the position of an element in the object can be used to access the element. Both strings and lists are ordered.


### Useful functions for list
// len() to calculate how many elements are there in the list, for example:
```
m=['a','d','v','g']
print(len(m))
4
```

//max() returns the greatest element in the list, for example: 
```
m=['a','d','v','g']
print(max(m))
v                     //The maximum elements in a list of strings is element that would occur last if the list were sorted alphabetically
```
//min() In the opposite way, returning the smallest element in the list.

//sorted() returns a copy of the list in order from smallest to biggest, for example:
```
m=['a','d','v','g']
print(sorted(m))
['a', 'd', 'g', 'v']
```

//join() is used to separate a list of strings with different elements, for example: 
```
a=['China','England','Russia','India']
print('\n'.join(a))
China
England
Russia
India
```
```
a=['China','England','Russia','India']
print(' '.join(a))
China England Russia India
```
```
a=['China','England','Russia','India']
print('\f'.join(a))
China
     England
            Russia
                  India

```

//append() is used to add an element to the end of the list, for example:
```
letters = ['a', 'b', 'c', 'd']
letters.append('z')            //an individual line of coding is needed to add 'z' to the end of the list. 
print(letters)
['a', 'b', 'c', 'd', 'z']
```

//how to **define a function(format is really important!)** to porcess operation, for example:
```
>>> a
[5, 6, 7, 8, 9, 0]
>>> def nba(a):               //define a copy function to operate the copy of a
...     a.copy()
...                           //empty this line to get the function start to work 
>>> nba(a)
>>> print(a)
[5, 6, 7, 8, 9, 0]

```

## Tuples: 
// Tuple is a data type for **immutable ordered** sequence of elements, in the form of **tuple( , ) or tuple ,**, for example:
```
tuple_a = 1, 2
tuple_b = (1, 2)
print(tuple_a == tuple_b)
True
```
```
location = (13.4125, 103.866667)
print("Latitude:", location[0]).  // similar to list, 
print("Longitude:", location[1])
```
// Tuples can be used to assign multiple variables in a compact way, for example: 
```
dimensions = 52, 40, 100
length, width, height = dimensions
print("The dimensions are {} x {} x {}".format(length, width, height))
The dimensions are 52 x 40 x 100
```

## Sets:
//data type for **mutable unordered** collections of unique elements, can be expressed in **brace brackets** 
// one application of sets is to remove duplicates from a list, **in sets, there is no repeating elements**, for example:
```
numbers = [1, 2, 6, 3, 1, 1, 6]
unique_nums = set(numbers)
print(unique_nums)
{1, 2, 3, 6}              
```

//Sets support the **in** operator the same as lists do. You can add elements to sets using the **add** method, and remove elements using the **pop** method,
```
fruit = {"apple", "banana", "orange", "grapefruit"}  // define a set
print("watermelon" in fruit)  // check for element
False                         // watermelon does not exist in the set so returns false.
```
```
fruit = {"apple", "banana", "orange", "grapefruit"} 
fruit.add("watermelon") // add an element
print(fruit)
{'grapefruit', 'orange', 'watermelon', 'banana', 'apple'}
```
```
fruit = {"apple", "banana", "orange", "grapefruit"} 
print(fruit.pop())  //remove a random element
print(fruit)
{'orange', 'watermelon', 'banana', 'apple'}
```

## Dictionaries
// dictionary **mutable, unordered** is composed of **key and value, input key, you can then get the value.**
// **the keys inside the dictionary can not be mutable type like list**, for example: 
```
room_numbers = {
    ['Freddie', 'Jen']: 403,
    ['Ned', 'Keith']: 391,
    ['Kristin', 'Jazzmyne']: 411,
    ['Eugene', 'Zach']: 395
}
```
output
```
Traceback (most recent call last):
  File "vm_main3.py", line 47, in <module>
    import main
  File "/tmp/vmuser_mjvldhtpbv/main.py", line 2, in <module>
    import studentMain
  File "/tmp/vmuser_mjvldhtpbv/studentMain.py", line 1, in <module>
    import dictionary_keys
  File "/tmp/vmuser_mjvldhtpbv/dictionary_keys.py", line 3, in <module>
    ['Freddie', 'Jen']: 403,
TypeError: unhashable type: 'list'
```

// mutable data type that stores mappings of unique keys to values (including strings, integers and floats) by **brace bracket**, for example:
``` 
elements = {"hydrogen": 1, "helium": 2, "carbon": 6}            
print(elements["helium"])            //print the value mapped to "helium"
2
```
```
elements= {"hydrogen": 1, "helium": 2, "carbon": 6}
elements[4]= 'dog'                   //insert key 4 with the value of 'dog' in the dictionary                
print(elements) 
{'hydrogen': 1, 'helium': 2, 'carbon': 6, 4: 'dog'}
```
// "in" can be used to check whether the elements are in the dictionary, returns True or False, for example: 
```
a={'Germany':4, 'China':5, 'United states':6 }
print("Britain" in a)
False
```
//"get" can be used to look up values in the dictionary, returns True or None, for example: 
```
a={'Germany':4, 'China':5, 'United states':6 }
print(a.get("dilithium"))
None
```

//new keys as well as their corresponding values can be added into dictionary, for example:
```
book_dict = {}
print("book_dict=", book_dict)
#add key value pairs
book_dict["vonnegut"] = "cat\'s cradle"
book_dict["ishiguro"] = "never let me go"
print("book_dict=", book_dict)
book_dict= {'vonnegut': "cat's cradle", 'ishiguro': 'never let me go'}
```

// Use **keys()** and **values()**, we can retrieve the keys or calues from the dictionary, for example: 
```
book_dict= {'vonnegut': "cat's cradle", 'ishiguro': 'never let me go'}
print(book_dict.keys())                             //retrieve keys from the dictionary. 
dict_keys(['vonnegut', 'ishiguro'])
print(book_dict.values())                           //retrieve values from the dictionary.
dict_values(["cat's cradle", 'never let me go'])
```

// use a **for loop** to iterate through the dict keys and values, for example:
```
book_dict= {'vonnegut': "cat's cradle", 'ishiguro': 'never let me go'}
>>> for key, value in book_dict.items():
...     print(key, ":", value)
... 
vonnegut : cat's cradle
ishiguro : never let me go
```


### Identity Operators
// You can check if a key returned None with the **is** operator. You can check for the opposite using **is not**, for example:
```
a={'Germany':4, 'China':5, 'United states':6 }
print(a.get("dilithium") is None).           //the result of "get" is none, using "is" to test it, we get True from the testing. 
True
```
```
a={'Germany':4, 'China':5, 'United states':6 }
print(a.get("dilithium") is not None)        //the result of "get" is none, using "is not" to test it, we get False from the testing.
False
```

// a default value can be set as a **return value** for "get", for example: 
```
a={'Germany':4, 'China':5, 'United states':6 }
a.get('kryptonite', 'There\'s no such element!')           // "There\'s no such element!" is the default value set for return. 
"There's no such element!"
```

//A more complicated example is given regarding dictionary, **list is embeded in the structure of dictionary**, for example:
```
animals = {'dogs': [20, 10, 15, 8, 32, 15], 'cats': [3,4,2,8,2,4], 'rabbits': [2, 3, 3], 'fish': [0.3, 0.5, 0.8, 0.3, 1]}
```

## Compound Data Structure
//We can include containers in other containers to create compound data structures,For example, **this dictionary maps keys to values that are also dictionaries**
```
elements = {"hydrogen": {"number": 1,
                         "weight": 1.00794,
                         "symbol": "H"},
              "helium": {"number": 2,
                         "weight": 4.002602,
                         "symbol": "He"}}
print(elements["hydrogen"]).                              // access the data "hydrogen" in the dictionary
{'number': 1, 'weight': 1.00794, 'symbol': 'H'}
```
//when a compound includes two or multiple dictionaries, we can access elements or add elements, for example:
```
elements = {'hydrogen': {'number': 1, 'weight': 1.00794, 'symbol': 'H'},
            'helium': {'number': 2, 'weight': 4.002602, 'symbol': 'He'}}

# todo: Add an 'is_noble_gas' entry to the hydrogen and helium dictionaries
# hint: helium is a noble gas, hydrogen isn't

elements['hydrogen']['is_noble_gas']= False.              // get into the dictionary's dictionary
elements['helium']['is_noble_gas']= True
print(elements['hydrogen']['is_noble_gas'])
print(elements['helium']['is_noble_gas'])
```

### Exercise 1 (how to convert a "string" to "list" then to "set") (from "list" to "set", repeating elements are excluded)
```
verse = "if you can keep your head when all about you are losing theirs and blaming it on you   if you can trust yourself when all men doubt you     but make allowance for their doubting too   if you can wait and not be tired by waiting      or being lied about  don’t deal in lies   or being hated  don’t give way to hating      and yet don’t look too good  nor talk too wise"
print(verse, '\n')

# split verse into list of words
verse_list = verse.split( )                          //split the string by blank----get the list
print(verse_list, '\n')

# convert list to a data structure that stores unique elements
verse_set = set(verse_list)                          //convert the list to set
print(verse_set, '\n')

# print the number of unique words
num_unique = len(verse_set)                          // get length of the set
print(num_unique, '\n')
```

### Exercise 2 (operation of dictionary and its derived operations)
```
verse_dict =  {'if': 3, 'you': 6, 'can': 3, 'keep': 1, 'your': 1, 'head': 1, 'when': 2, 'all': 2, 'about': 2, 'are': 1, 'losing': 1, 'theirs': 1, 'and': 3, 'blaming': 1, 'it': 1, 'on': 1, 'trust': 1, 'yourself': 1, 'men': 1, 'doubt': 1, 'but': 1, 'make': 1, 'allowance': 1, 'for': 1, 'their': 1, 'doubting': 1, 'too': 3, 'wait': 1, 'not': 1, 'be': 1, 'tired': 1, 'by': 1, 'waiting': 1, 'or': 2, 'being': 2, 'lied': 1, 'don\'t': 3, 'deal': 1, 'in': 1, 'lies': 1, 'hated': 1, 'give': 1, 'way': 1, 'to': 1, 'hating': 1, 'yet': 1, 'look': 1, 'good': 1, 'nor': 1, 'talk': 1, 'wise': 1}
print(verse_dict, '\n')

# find number of unique keys in the dictionary
num_keys = len(verse_dict)
print(num_keys)

# find whether 'breathe' is a key in the dictionary
contains_breathe = verse_dict.get('breathe')
print(contains_breathe)

# create and sort a list of the dictionary's keys
sorted_keys = verse_dict.keys()
sorted_keys = sorted(sorted_keys)
print(sorted_keys)
# get the first element in the sorted list of keys
print(sorted_keys[0])

# find the element with the highest value in the list of keys
print(sorted_keys[-1]) 
```

## Summary of Datastructure 
![Screen Shot 2022-03-08 at 5 22 26 PM](https://user-images.githubusercontent.com/100081406/157282172-835b4d1b-66cd-4923-bcd2-dda759fbfd4d.png)


 
# Control flow 
## Conditional Statements
### if statement
// if statement is a conditional statement that runs or skips code based on whether a condition is true or false, for example: 
```
>>> bank_balance= 3                         //it is important to define first before starting if statement
>>> phone_balance = 4
>>> if phone_balance < 5:
...     phone_balance += 10
...     bank_balance -= 10
...                                         //empty one line to quit the if statement 
>>> bank_balance 
-7
>>> phone_balance 
14
```

// the combination of **if, elif and else** can help to print the result, **elif can be multiple but only one else** for example:
// for if statements, **we can use 'if' only, 'if' and 'elif', 'if' and 'else', and 'if', 'elif' and 'else' all together. **3
```
>>> season = 'winter'
>>> if season == 'spring':
...     print('plant the garden!')
... elif season == 'summer':                    
...     print('water the garden!')
... elif season == 'fall':
...     print('harvest the garden!')
... elif season == 'winter':
...     print('stay indoors!')
... else:                                                  //there is no conditiuon should be added for else!!!!!
...     print('unrecognized season')
... 
stay indoors!
```

### for loop
// for() is used to iterate elements, for example: 
```
>>> cities={'Qingdao','Shanghai','Beijing'}
>>> for city in cities:
...     print(city)
... 
Shanghai
Beijing
Qingdao
```

//use the range() function 








