# Python-code

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
output;
```
['Milk', 'Chicken', 'Bread, Butter']
['Milk', 'Chicken, Bread, Butter']
['Milk', 'Chicken', 'Bread', 'Butter']
['Milk, Chicken, Bread, Butter']
```























