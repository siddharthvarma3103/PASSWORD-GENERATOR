# PASSWORD-GENERATOR
import random
import string
lcase=string.ascii_lowercase
ucase=string.ascii_uppercase
l_num=[1,2,3,4,5,6,7,8,9,0]
l_uchar=list(ucase)
l_lchar=list(lcase)
l_spl=["@","!","#","$","^"]
passw=random.choice(l_uchar)+random.choice(l_lchar)+str(random.choice(l_num))+random.choice(l_spl)
k=[1,2]
x=random.choice(k)
if(x==1):
    passw+=random.choice(l_uchar)+random.choice(l_uchar)+random.choice(l_lchar)+random.choice(l_lchar)
else:
    passw+=random.choice(l_lchar)+random.choice(l_lchar)+str(random.choice(l_num))+str(random.choice(l_num))
m=[8,9,10]
y=random.choice(m)
if(y==8):
    print(passw)
elif(y==9):
    passw+=random.choice(l_spl)
    print(passw)
else:
    passw+=random.choice(l_spl)+random.choice(l_uchar)
    print(passw)
