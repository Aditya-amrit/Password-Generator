# Password-Generator

print("WELCOME TO STRONG PASSWORD GENERATOR")

import random

Alp=['a','A','b','B','c','C','d','D','e','E','f','F','g','G','y','Y','z','Z']
sym=['!','@','$','#','%','^','&','*','~']
num=['1','2','3','4','5','6','7','8','9','10']

a=int(input("How many Alphabets do you want: "))
b=int(input("How many symbols do you want: "))
C=int(input("How many number do you want: "))

password = ""
for a in range(0,a):
    password += random.choice(Alp)
for b in range(0,b):
    password += random.choice(sym)
for c in range(0,C):
    password += random.choice(num)

print(password)

e=list(password)
random.shuffle(e)
password=''.join(e)

print(f"Your Password is: {password}")
