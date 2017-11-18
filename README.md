# Besic-python-code-
#1. Write a code to find string after $5 from string. String is " i have $2 in my pockets and $5 in wallet and i need $3 more "

str1 = " i have $2 in my pockets and $5 in wallet and i need $3 more "
'''str2 = str1.split()
str3=(str2[8:14])
str4 = ' '.join(map(str, str3))
print(str4)
#	or
print(str1[31:61])
'''

#2. Write the code to Initialize a dictionary in python and save data of the dictionary in a file?
#using json
'''
data = {}
data ['key1'] = "keyinfo"
data ['key2'] = "keyinfo2"

import json
with open('data.json', 'w') as fp:
    json.dump(data, fp)

#using piclke
import cPickle as pickle
with open('data.p', 'wb') as fp: #save
    pickle.dump(data, fp)
with open('data.p', 'rb') as fp: #load
    data = pickle.load(fp)
'''

#3. Write a code to Read a file and append lines to a list?
'''
file1 = ["Mannu","python"]
import json
with open ('New_file.json','w') as fp:
	json.dump(file1,fp)
file1.append('java')
with open ('New_file.json','w') as fp:
	json.dump(file1,fp)
'''
#4. Write a program to give each output of list is multiply by 2
'''
a = [2,4,6,8]
z = []
for i in a:
	x=i*2
	z.append(x)
print(z)
'''
#5. Write a code to catch an Exception in python.
'''
try: 
    x = int(input("Enter 1st number : "))
    y = int(input("Enter 2nd number : ")) 
    z = x / y  
    print ("--> z=%d" % (z))
except: 
    print ("Values at Exception: x=%d y=%d " % (x,y)) 
    print ("The error was on line ..." )
    print ("The reason for the error was ... y must be grather than 0")
'''
#6. How to convert string to lowercase in Python?
'''
str1 = (input("Enter your name : "))
print(str1.lower())
'''
#7. Write a function which takes input as a list of elements and merge all strings separated by '#' and add all numbers. Handle exceptions
'''
list1 = []
def insert(x):
	list1.append(x)
for i in range(5):
	i = (input("Enter your name : "))
	insert(i) 
	print(list1)
	str1 = '#'.join(map(str, list1))
	print(str1)
'''

#8. Write a script to sort a dictionary based on its values.
'''
dict1 = {'age0':'20','age1':'21','age2':'22','age3':'23','age4':'24'}
for k, v in dict1.items():
	print "%s: %s" % (v, k)
'''
#11. How to iterate over a dict in python?
'''
dict1 = {'age0':'20','age1':'21','age2':'22','age3':'23','age4':'24'}
it=iter(dict1)
print(it.next())
print(dict1.items())
'''
#13. Define list of tuples with size 4.
'''
x = [1, 2, 3, 4]
y = ['a','b','c','e']
zipped = zip(x, y)
print(zipped)
'''

#14. Write a program for function overriding and function overwriting.

#15. Write a code to reverse the string by words. str1 = "NLP & ML"
str1 = "NPL & ML"
a =str1.split()
print(a)
z=a[::-1]
print(z)
b=' '.join(map(str, z))
print(b)
