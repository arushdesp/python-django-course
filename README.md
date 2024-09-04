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
