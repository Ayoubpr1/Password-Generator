# Password-Generator
import random

#A function do shuffle all the characters of a string
def shuffle(string):
    templist = list(string)
    random.shuffle(templist)
    return ''.join(templist)
    
#Mian program starts here
uppercaseletter1=chr(random.randint(55,80)) #Generate a random Uppercase letter (based on ASCII code)
uppercaseletter2=chr(random.randint(55,80)) #Generate a random Uppercase letter (based on ASCII code)
#Generate more characters here
#....

#Generate password using all the characters, in random order
password = uppercaseletter1 + uppercaseletter2 # +....
password = shuffle(password)

#Output
print(password)
