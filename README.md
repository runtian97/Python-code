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
a = 'I wanna quit my PhD' 
print(a)
I wanna quit my PhD

// if there is already quotes in the strings, then back slash is needed, example: 
b = "Simon\'s skateboard is in the garage"
print(b)
Simon's skateboard is in the garage

// "+" can be used to combine two strings, examlpe: 
a = "hello"
b = "world"
print(a+" "+b)
hello world

// "*" can be used to repeat the stings, examples:
a = "jeremy"
print((a+" ")*5)
jeremy jeremy jeremy jeremy jeremy 

// "len" can be used to count the length of a string, example:
a="jeremy"
print(len(a))
6
b = "luterbacher"
print(len(a)/len(b))
0.5454545454545454

//"[]" can be used to check out the alphabet or number at different locations of the string (always [0] indicates the first one of the string), example:
a = 'lebron'
>>> a[0]
'l'


## Integer, floats and 
// use type to recognize the types of number, example:
type(5.6)
<class 'float'>

// type can be changed, example: 
a=6.5
>>> int(a)
6
>>> float(a)
6.5
>>> str(a)
'6.5'

## string methods: always called with dot 
// "title" can be used to capitalize the name, example: 
print ("china gao".title()) // 
China Gao











