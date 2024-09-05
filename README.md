# python-django-course

Basically a user will request a url from our website. It goes to the urls.py which is going to the view.py to django from a call that goes to the models.py that has the database information which is feeded back to the models.py views,py which is going to the templates containing the htmls,css,js and returns to the user.

## Level 1 
mystring = 'abcdefg'
print(mystring[:3]) ## result abc starts from 0
print(mystring[2:5]) ## resiòt cde
print(mystring[::]) ## entire string
print(mystring[::2]) ## jumps two everytime

mystring = 'Hello World'
x = mystring.split()
print(x) ['Hello','World']

Print formatting 
x = "Item One: {x} Item Two {}".format(x="dog",y="cat")
print(x) ## Items One: cat Items Two: dog

## Lists
mylist = ['a','b','c','d']
print('before reassignment:')
print(mylist)
mylist[] = 'New Item'
print("after reassignment:") ### New List,b,c,d

mylist = ['a','b','c','d']
listtwo = ["x",'y','z']
mylist.append(["x",'y','z'])
Result: a,b,c,d,[x,y,z]
mylist.extend(listtwo)
print(mylist) ## a,b.c.d.x.y.z

mylist = ['a','b','c','d','e']
item = mulist.pop() ## will be the last one unless we indicate
print(mylist)
print(item)

mylist = ['a','b','c','d','e']
mylist.reverse()
print(mylist)

mylist = [4,5,6,7,8,34,3,8]
mylist.sort()
print(mylist)

matrix = [[1,2,3],[4,5,6],[7,,8,9]]
first_col = [row[0] for row in matrix]
print(first_col) ## [1,4,7]

## Dictionaries: key-value pairs it is not ordered
my_stuff = {"key1":"value"."key2:'value2'}
print(mystuff['key2']) ## printed value2
e.g. 
my_stuff = {"key1":"value"."key2:'value2','key3':{1,2,'grabMe']}}
print(my_stuff['key3']['123'][2].upper()) result: grabMe GRABME with upper

my_stuff = {'lunch':'pizza','bfast':'eggs'}
print(mystuff['lunch']

we cna change it like:
mystuff['lunch'] = 'burger'
print(my_stuff['lunch'] ## result burger

tuples are immutables. booleans are true and false statements.
## Booleans True or False or 0 or 1
t = (1,2,3)
print(t[0]) ##result 1
t = ('a',True.123)
print(t)
t[0] = ' NEW ' error and it cant change lists [] tuples ()

## Sets.
x = set()
x.add(1)
x.add(2)
print(x) ### {1,2} no particular order in a set

converted = set([1,2,3,3,3])
[1,2,3]

## Problems.
Given the string s = 'django'
print the following, 'd','o','djan','jan'
s[0] - 'd'
s[5] - 'o'
s[:4] - djan
s[1:4] - jan
reverse the string s[::-1]

l = [3,7,[1,4,'hello']]
l[2][2] = 'goodbye'

d3 = {'k1':[{'nest_key':['this is deep',['hello']]}]}
d3[k1][0]['nst_key'][1][0]
grab the "hello"

age = 4
name = "Sammy"

"Hello my dogs name is Sammy and he is 4 years old"

print("Hello my dogs name is {a} and he is {b} years old".format(a=age,b=name))

## Control Flow operators if/else if/else

Comparison operations no type coersion as in js
=> == != <= 
1>2 and 2<3
1>2 or 2<5
If else.
if 1<2: (then : )
  print('yes')


if 1<2:
  print("Hello")
else:
  print('last')

seq = [1,2,3,4,5]

for item in seq:
  print(item) # prints 1,2,3,4,5,6
  print('Hello') #prints Hello >>>>>


d = {"Sam":1,"Frank",2,"Dan":3}
for item in d:
  print(item)
  print(d[item])

mypairs = [(1,2),(3,4)(5,6)]

for item in mypairs:
  print(item)

for (tup1,tup2) in mypairs:
  print(tup2)
  print(tup1)


i = 1
while i<5
  print("i is: {}".format(i))
  i = i+1
range(5) => range(0,5)
list(range(0,5)) to a list [0,1,2,3,4,5]

list(range(0,11,2))
0,2,4,5,6,8,10

for item in range(10):
  print(item)

x = [1,2,3,4]
out = []

for num in x:
  out.append(num**2)
print(out)
OR 
out = [num**2 for num in x]
print(out)

def my_func(param1='default')
  print("my first pfunction".format(param1))
my_func()

def my_func(param1='default')
  """
  This is the docstring
  """
  print("my first python function {}".format(param1)



def hello():
  print("hello")
result = hello()
print(result)

def addNum(num1,num2):
  return num1+num2
result = addNum(2,3)

def addNum(num1,num2):
  if type(num1)==type(num2)==type(10):
    return num1+num2
  else
    return "sorry I need integers"

result = addNum(2,3)
print(type(result))

mylist = [1,2,3,4,5,6,7,8]
def even_bool(num):
  return num%2 == 0
evens = filter(even_bool,mylist)
print(list(evens)) # prints a list of the evens function with the my list list

mylist = [1,2,3,4,5,6,7,8]
events =filter(lambda num:num%2 == 0,mylist)
print(list(events))

tweet = "go sports! #sports"
result = tweet.split('#') [1] ## split it into a list and take the 2on part of the list after the #
print(result)

class Dog:
    # Class attribute
    species = 'Canis familiaris'

    # Constructor method
    def __init__(self, name, age):
        # Instance attributes
        self.name = name
        self.age = age

    # Method (function inside a class)
    def description(self):
        return f"{self.name} is {self.age} years old."

    # Another method
    def speak(self, sound):
        return f"{self.name} says {sound}."

# Create an instance of Dog class
my_dog = Dog("Buddy", 3)

# Access attributes and call methods
print(my_dog.description())  # Buddy is 3 years old.
print(my_dog.speak("Woof!"))  # Buddy says Woof!
Key Concepts
__init__ Method (Constructor): Initializes the object when it's created. It allows setting the initial state of the object.

Attributes: Variables that belong to the object. Attributes can be defined inside the __init__ method or can be shared across all instances (class attributes).

Methods: Functions defined inside a class that perform actions using the object’s attributes. Methods usually operate on the object itself.

Inheritance
Inheritance allows one class (child class) to inherit attributes and methods from another class (parent class).

class Animal:
    def __init__(self, name):
        self.name = name

    def speak(self):
        raise NotImplementedError("Subclasses must implement this method")

# Inherit from the Animal class
class Cat(Animal):
    def speak(self):
        return f"{self.name} says Meow!"

class Dog(Animal):
    def speak(self):
        return f"{self.name} says Woof!"

# Create instances of Cat and Dog
my_cat = Cat("Whiskers")
my_dog = Dog("Fido")

print(my_cat.speak())  # Whiskers says Meow!
print(my_dog.speak())  # Fido says Woof!

Key Features of Inheritance:
Superclass (Parent Class): The class whose methods and attributes are inherited.
Subclass (Child Class): The class that inherits from the superclass. It can override or extend the functionality of the superclass.
Method Overriding: A subclass can provide a specific implementation of a method that is already defined in its superclass.

Encapsulation
Encapsulation is about restricting direct access to certain attributes and methods, and it can be achieved using private attributes (prefixing them with __).

class Car:
    def __init__(self, model, year):
        self.__model = model  # Private attribute
        self.year = year

    def get_model(self):
        return self.__model

# Accessing a private attribute through a getter method
my_car = Car("Tesla", 2020)
print(my_car.get_model())  # Tesla


Polymorphism
Polymorphism allows the same method to be used for different object types. For example, different classes may define their own speak() method, but you can use them interchangeably.

for animal in [my_dog, my_cat]:
    print(animal.speak())


Abstraction
Abstraction hides complex implementation details and exposes only the necessary parts. In Python, abstraction is achieved through abstract base classes (ABC), requiring subclasses to implement specific methods.

from abc import ABC, abstractmethod

class Shape(ABC):
    @abstractmethod
    def area(self):
        pass

class Rectangle(Shape):
    def __init__(self, width, height):
        self.width = width
        self.height = height

    def area(self):
        return self.width * self.height

rect = Rectangle(5, 10)
print(rect.area())  # 50
Summary
Class: A blueprint for objects.
Object: An instance of a class.
Attributes: Variables defined in the class.
Methods: Functions that operate on the attributes.
Inheritance: Allows a class to inherit behavior from a parent class.
Encapsulation: Hides the internal representation of the object.
Polymorphism: The same operation works differently on different classes.
Abstraction: Focuses on essential qualities rather than specific details.
