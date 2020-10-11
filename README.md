# Assignment-5-Exception-Handling_Data-Science

#Write a function to compute 5/0 and use try/except to catch the exceptions.

def DivideByZero(x,y):
    try:
        x/y
    except ZeroDivisionError as e:
        print("An interger/number can't be divisible by Zero")
        print("An execption has been occured as, ",e, " action has been attempted")

# apply values on variable x & y
x,y=5,0

#Function Execute
DivideByZero(x,y)

output
An interger/number can't be divisible by Zero
An execption has been occured as,  division by zero  action has been attempted

# 2. Implement a Python program to generate all sentences where subject is in 
#["Americans","Indians"] and verb is in ["Play", "watch"] and the object is in ["Baseball","cricket"].
            #Hint: Subject,Verb and Object should be declared in the program as shown below.
                   #subjects=["Americans ","Indians"] verbs=["play","watch"] objects=["Baseball","Cricket"]
                #Output should come as below:
                #Americans play Baseball. Americans play Cricket.
                #Americans watch Baseball. Americans watch Cricket. 
                #Indians play Baseball. Indians play Cricket. 
                #Indians watch Baseball. Indians watch Cricket.

#solution:-

subject=["Americans","Indians"]
verb=["play","watch"]
objects=["Baseball","Cricket"]
# List Comprehension  #for Loop for Iteration
Syntax = [(Sub+' '+vrb+' '+Objct+".") for Sub in subject for vrb in verb for Objct in objects]
print("Output:")
for syn in Syntax:    
    print(syn)


Output:
Americans play Baseball.
Americans play Cricket.
Americans watch Baseball.
Americans watch Cricket.
Indians play Baseball.
Indians play Cricket.
Indians watch Baseball.
Indians watch Cricket.
