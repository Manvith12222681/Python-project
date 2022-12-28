# Python-project
In this project you have to enter a range [A, B] and system will randomly pick any number from your  given range and check the status of the given numbers.



A =int(input('''Enter the starting of range : '''))
B =int(input('''Enter the ending of range : '''))
import random
a = random.randint(A,B)
print('''
        random number is ''', a)
if a%2==0:
    print('''
        it is even''')
else:
    print('''
        it is odd''')
if a<0:
    print('''
        its negative ''')
else:
    print('''
        its positve''')
    
count = 0
if a>1:
    for i in range(2,(a//2+1)):
        if (a%i)==0:
            count=count+1
            break
    if(count==0 and a!=1):
        print('''
         The given number''',a,'''is prime''')
    else:
        print('''
        The given number''',a,'''is composite''')
else:
    print('''
        negative numbers are neither prime nor composite''')
    
    
    
