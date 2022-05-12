- # -*- coding: utf-8 -*-
"""
Created on Fri Apr 29 18:14:35 2022

@author: Mehul
"""

'Slips'
 
'''Slip 1: Pattern Program

1
2 3
4 5 6
7 8 9 10'''

# rows=4
# n=1
# for i in range(0,rows):
#     for j in range(0,i+1):
#         print(n,end="  ")
#         n=n+1  
#     print(' ')  
    
'''Slip 2: Write a python program to accept string and remove the characters which 
have odd index values of given string using user defined function.'''

str=input("\n Enter a string :")
def remov(str):
    i=0
    new_str=''
    while i<len(str):
        new_str+=str[i]
        i+=2
    return new_str


print(remov(str))

'Slip 3: Write a program to check whether a number is armstrong or not'

# n= int(input("Enter the number : "))
# number = n
# sum = 0
# power = len(str(n))

# while(n>0):
#     digit = n % 10
#     sum += digit **power
#     n = n//10

# if(sum == number):
#     print("ARMSTRONG NUMBER")
# else:
#     print("NOT AN ARMSTRONG NUMBER")

'''Slip 4: Write a python function that accepts a string and calculate
the number of upper case letters and lower case letters'''

def case_string(str):
    up_count=0
    low_count=0
    for i in str:
        if(i.isupper()):
            
            up_count+=1
        elif(i.islower()):
                
            low_count+=1
    print("Number of upper case characters ",up_count)
    print("Number of low case characters ",low_count)
str=input("\nEnter a string :")
case_string(str)

'Slip 5: Write a program to reverse a string'

# txt = str(input("\nEnter the String to be reversed: "))
# reverse = txt[::-1]
# print(reverse)

'''SLip 6: Write a Python program to check if a given key already exists in a dictionary. 
If key exists replace with another key/value pair.'''

# d={'apple':200,'pear':250}
# if 'pear' in d:
#     d['orange']=d.pop('pear')
#     d['orange']=100
# print(d)

'''Slip 7: Write a Python Program to Check if given number is prime or not.
 Also find factorial of the given no using user defined function.'''
 
 #num=int(input("\nEnter the number : "))
 #flag=0
 #for i in range(2,num):
 #    if(num%i)==0:
 #        flag=1
 #        break
 #if(flag==1):
 #    print(num,"is not a prime number")
 #else:      
 #    print(num,"is a prime number")
     
 #def fact(n):
 #    if(n==0):
 #       
 #        f=1
 #        
 #    f=1    
 #      
 #    for i in range(1,n+1):
 #        
 #        f=f*i
 #        
 #    return f
 #num=int(input("\n Enter the number : "))
 #ff=fact(num)
 #print("factorial of",num,"is",ff)

 
'''Slip 8: Write a python script to define a class student having members roll no, name, age, gender.
 Create a subclass called Test with member marks of 3 subjects.
 Create three objects of the Test class and display all the details of the student with total marks.''' 
 
 # class Student:
 #     def GetStudentInfo(self):
 #         self.rollno=int(input("Enter the roll no: "))
 #         self.name=input("Enter the name: ")
 #         self.age=int(input("Enter the age: "))
 #         self.gender=input("Enter the gender: ")
         
 #     def display(self):
 #         print(self.rollno)
 #         print(self.name)
 #         print(self.age)
 #         print(self.gender)
         
 # class Test(Student):
 #     def GetMarks(self):
 #         self.m1=int(input("Enter m1:"))
 #         self.m2=int(input("Enter m2:"))
 #         self.m3=int(input("Enter m3: "))
         
 #     def displaydata(self):
 #         print("Marks of 1st subject : ", self.m1)
 #         print("Marks of 2nd subject : ", self.m2)
 #         print("Marks of 3rd subject : ", self.m3)
 #         print("Total: ", self.m1+self.m2+self.m3)
         
 # n=int(input("Enter how many students :"))
 # s=[]
 # for i in range(0,n):
 #     x=input("Enter obj name: ")
 #     s.append(x)
 #     print(x)
     
 # for j in range(0,n):
 #     s[j]=Test()
 #     s[j].GetStudentInfo()
 #     s[j].GetMarks()
     
 # for j in range(0,n):
 #     s[j].display()
 #     s[j].displaydata()
 
 
'Slip 9: Write an anonymous function to find area of square and rectangle.'

# s=int(input("Enter a side:"))
# square=lambda s: s*s
# print("Area of square : ",square(s))

# l = int(input("Enter length :"))
# b = int(input("Enter breadth :"))
# rectangle=lambda l,b:l*b
# print(":Area of rectangle: ",rectangle(l,b))  


'''Slip 10: Write Python script to create 2 text files. 
Enter data in each file and merge the data in the third file. (using function).'''

# def program2():
#     mf = open("myfile.txt","w")
#     line1 = input ("Enter line 1: ")
#     mf1 = open("myfile1.txt","w")
#     line2 = input("Enter line2:")
    
#     mf.write(line1)
#     mf1.write(line2)
#     mf.close()
#     mf1.close()
# program2()

# def program3():
#     with open("myfile.txt","r")as f1:
#         data = f1.read()
#     with open("myfile1.txt","r")as f2:
#         data1 = f2.read()
#     with open("merge.txt","w")as f3:
#           f3.write(data)
#           f3.write(data1)
#     f1.close()
#     f2.close()
#     f3.close()
# program3()
# str = open("merge.txt","r")
# s = str.read()
# print(s)      


'''Slip 11: Create a list a = [1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89] and write a python program that 
prints out all the elements of the list that are less than 5.'''

# a=[1,1,2,2,3,4,15,16,7,8,9]
# print(a)
# for i in a:
#   if i<5:
#     print(i)    

 
'''Slip 12. Write a Python class which has two methods get_String and print_String. 
get_String accept a string from the user and print_String print the string in upper case.
Further modify the program to reverse a string word by word and print it in lower case.'''

# class String:
#     def get_String(self):
#         self.str=input("Enter a string: ")
#     def print_String(self):
#         print(str.upper(self.str))
#     def reverse(self):
#         str1=self.str[ : :-1]
#         print(str.lower(str1))

# Obj=String()
# Obj.get_String()
# Obj.print_String()
# Obj.reverse()


'''Slip 13: Write a Python program to accept n numbers in list and remove duplicates from a list.'''

# a=int(input("How many numbers do you want to enter?"))
# l=[]
# for i in range(a):
#         l.append(int(input("Enter a number ")))
# print("The original list is:", l)

# new=[]
# for x in l:
#     if x not in new:
#         new.append(x)
# print("The list with no duplication is: ",new)


'''SLip 14: Write a python script to define the class person having members name, address.
Create a subclass called Employee with member salary.
Create 'n' objects of the Employee class and display all the details of the employee.'''
        
# class Person:
#     def AcceptPerson(self):
#         self.name=input("Enter Name:")
#         self.address=input("Enter Address:")
        
#     def DisplayPerson(self):
#         print("Name:",self.name)
#         print("Address",self.address)
        
# class Employee(Person):
#     def AcceptSal(self):
#         self.salary=input("Enter Salary:")
#     def DisplaySal(self):
#         print("Salary:",self.salary)

# m=int(input("Enter How many Employees:"))     
# s=[]
# for i in range(m):
#     x=input("Enter Object Name:")
#     s.append(x)
# for j in range(m):
#     s[j]=Employee()
#     s[j].AcceptPerson()
#     s[j].AcceptSal()
# for j in range(m):
#     s[j].DisplayPerson()
#     s[j].DisplaySal()    



'''SLip15: Write a program that encrypts a message by adding a key value to every character.'''

# message=input("Enter a string:")
# index=0
# while index<len(message):
#     ch=message[index]
#     print(chr(ord(ch)+3),end=' ')
#     index+=1
    
'''Slip 16: Write a Python script using class, which has two methods get_String and print_String. 
get_String accept a string from the user and print_String print the string in upper case.'''

# class String:
#     def get_String(self):
#         self.str=input("Enter a string: ")
#     def print_String(self):
#         print(str.upper(self.str))

# Obj=String()
# Obj.get_String()
# Obj.print_String()


'''Slip 17: Write a python script to find the repeated items of a tuple. tup=(1,2,2,3,4,4)'''

# T=(2,2,2,2,4,4,4,5,5,7,8,9)
# T1=()
# for i in T:
#     if(T.count(i)>1):
#         if i not in T1:
#             new_ele=(i,)
#             T1=T1+new_ele
# print(T1)            


'''Slip 18. Write a python program to count repeated characters in a string.
Sample string: 'thequickbrownfoxjumpsoverthelazydog
Expected output: o-4, e-3, u-2, h-2, r-2, t-2'''

# string = "thequickbrownfoxjumpsoverthelazydog"

# print("Duplicate characters in a given string: ")
# #Counts each character present in the string
# for i in range(0, len(string)):
#     count=1
#     for j in range(i+1, len(string)):
#         if(string[i]== string[j] and string[i] != ' '):
#             count += 1
            
#             string = string[:j] + '0' + string[j+1:]
            
# # A character is considered as duplicate if count is greater than 1            
#     if(count > 1 and string[i] != '0'):
#         print(string[i], count)  


'''Slip 19: Write a program to implement the concept of queue using list.'''

# queue=[1,2,3,4,5]
# print(queue)
# queue.append(6)
# print("Queue after insertion is: ",queue)
# queue.pop(0)
# print("Queue after deletion is: ",queue)


'''Slip 20: Write a python program to count number of upper case letters, small case letters,
 digits in the file.'''

# f = open("merge.txt","r")
# s = f.read()
# cntu,cnts,cntd = 0,0,0
# for ch in s:
#     if ch.isupper():
#         cntu+=1
#     elif ch.islower():
#         cnts+=1
#     elif ch.isdigit():
#         cntd+=1
# print("No. of Upper case letters: ",cntu)
# print("No. of Lower case letters: ",cnts)  
# print("No. of digits: ",cntd)      

'''Slip 21: Write a program that counts the number of occurrences of a character in a string.'''

# def count_char(s,c):
#     count = 0
#     for i in s:
#         if (i==c):
#             count+=1
#     return count
# str= input("\n Enter a string : ")
# ch=input("\n Enter the character to be searched : ")
# count=count_char(str,ch)        
# print("In" ,str,ch,"occurs", count, "times")


'''Slip 22: Write a Pickle python program to write and read a data from a file stating the position of the file object.
(Using dump(), load() functions).'''


'''Slip 23: Write a Python script to generate and print a dictionary which contains 
a number (between 1 and n) in the form(x,x*x).
Sample Dictionary (n=5) Expected Output: {1:1, 2:4, 3:9, 4:16, 5:25}'''

# n=int(input("Enter a number:"))
# Dict={x: x*x for x in range(1,n+1)}
# print(Dict)


'''Slip 24: Write a file handling program in python, which opens the file ‘report.txt’ and write data into it.
Use the seek() and tell() functions in python while reading the data from the file.'''


'''Slip 25: Write a python script to implement bubble sort using list.'''

# list1=[5,2,9,4,3,1]
# print("The Unsorted List is:",list1)

# for i in range(0,len(list1)-1):
#     for j in range(len(list1)-1):
#         if(list1[j]>list1[j+1]):
#             temp=list1[j]
#             list1[j]=list1[j+1]
#             list1[j+1]=temp
# print("The Sorted List is:",list1)


'''Slip 26: Write a python script to create a class Rectangle with data member’s length, width and methods area,
 perimeter which can compute the area and perimeter of rectangle.'''
 
 
'''Slip 27. Write a Python program to convert a tuple of string values to a tuple of integer values.
Original tuple values: (('44', '444'), ('1516', '45')) New tuple values: ((44, 444), (1516, 45))'''

# tup_str = (('44','444'),('1516','45'))
# print("Original tuple values are:" ,tup_str)
# tup_int=tuple((int(x[0]), int(x[1])) for x in tup_str)
# print("\n New tuple values:" ,tup_int)


'''Slip 28: Write a python program to fully reverse the contents of file and write it in another file.'''


'''Slip 29: Write a Python program to accept two lists and merge the two lists into list of tuple.'''

# list1=[]
# list2=[]

# n1=int(input("How many elements to enter for list1 ?? "))
# for i in range(n1):
#     elements1=int(input("Enter the elements : "))
#     list1.append(elements1)
    
# n2=int(input("How many elements to enter for list2 ?? "))    
# for i in range(n2):
#     elements2=int(input("Enter the elements : "))
#     list2.append(elements2)
    
# print(list1,list2)

# new_list=list(zip(list1,list2))
# print(new_list)


'''Slip 30: Write a python program to create a class Circle and compute the Area and the circumferences of the circle.
(use parameterized constructor)'''

# import math
# class Circle():
#     def __init__(self,radius):
#         self.radius=radius
        
        
#     def area(self):
#         return math.pi*(self.radius**2)
    
#     def circumference(self):
#         return 2*math.pi*self.radius
# r=int(input("Enter radius of circle: "))
# obj=Circle(r)
# print("Area of circle: ",round(obj.area(),2))
# print("Circumference of circle: ",round(obj.circumference(),2))


'''Slip 31: Write a Python script to sort (ascending and descending) a dictionary by key.'''

# D={1:10,5:20,2:54,3:987,10:432}
# for key in sorted(D.keys ()):
#     print ("D[",key,"]:",D[key])
# for key in sorted(D.keys (),reverse=True):
#     print ("D[",key,"]:",D[key])


'''Slip 32: Define a class named Shape and its subclass Square. 
The subclass has an init function which takes an argument Length. 
Both classes should have methods to calculate area and perimeter of a given shape.'''

# class Shape():
#     def __init__(self):
#         pass
    
#     def area(self):
#         raise NotImplementedError
#     def perimeter(self):
#         raise NotImplementedError

# class Square(Shape):
#     def __init__(self,l):
#         self.length=l
#     def area(self):
#         return self.length*self.length
#     def perimeter(self):
#         return 4*self.length
# aSquare=Square(3)
# print("Area: ",aSquare.area())
# print("Perimeter: ",aSquare.perimeter())


'''Slip 33: Write a Python program to unzip a list of tuples into individual lists.'''

# l = [(1,2), (3,4), (8,9)]

# #map(list, zip(*L))
# [list(t) for t in zip(*l)]


'''SLip 34: Write Python program that has a class Person storing name and date of birth(DOB) of a person.
 Subtract the DOB from today’s date to find out whether a person is eligible to vote or not.'''
 
# import datetime
# class Person():
#     def __init__(self,name,dob):
#         self.name=name
#         self.dob=dob
#     def check(self):
#         today=datetime.date.today()
#         print("today: ",today)
#         age=today.year-self.dob.year
        
#         if age>=18:
#             print("Eligible")
#         else:
#             print("Not Eligible")
# p=Person("ss",datetime.date(2008,12,11))
# p.check()            
            

'''Slip 35: Write a Python program to compute element-wise sum of given tuples.
Original tuples: (1, 2, 3, 4) (3, 5, 2, 1) (2, 2, 3, 1)
Element-wise sum of the said tuples: (6,9,8,6).(map funct)'''

# def add(x,y,z):
#     return x+y+z
# tup1=(1,2,3,4)
# tup2=(2,3,4,5)
# tup3=(2,2,1,6)
# tup4=tuple(map(add,tup1,tup2,tup3))
# print(tup4)


'''SLip 36: Define a class Employee having members id, name, department, salary. 
Create a subclass called manager with member bonus.Define methods accept and display in both the classes.
 Create n objects of the manager class and display the details of the manager having the maximum total salary (salary+bonus).'''
 
# class Employee:
#      def EmployeeInfo(self):
#          self.__id=input("enter id: ")
#          self.__name=input("Enter the name: ")
#          self.sal=int(input("Enter the sal: "))
#          self.__dept=input("Enter the dept: ")
         
#      def PrintInfo(self):
#          print("id:",self.__id,"name:",self.__name)
            
             
# class Manager(Employee):
#      def ManagerInfo(self):
#              Employee.EmployeeInfo(self)
#              self.__bonus=int(input("Enter a bonus: "))
             
#      def PrintManagerInfo(self):
#             Employee.PrintInfo(self)
#             self.TotalSalary=self.__bonus+self.sal
#             print("Total Salary: ", self.TotalSalary)
             
# n=int(input("Enter how many Managers :"))
# s=[]
# for i in range(0,n):
#      x=input("Enter obj name: ")
#      s.append(x)
#      print(x)
         
# for j in range(0,n):
#      s[j]=Manager()
#      s[j].ManagerInfo()
         
         
# for j in range(0,n):
#      s[j].PrintManagerInfo()
         
# maxTotalSalary=s[0].TotalSalary       
# maxIndex=0
# for j in range(1,n):
#      if s[j].TotalSalary>maxTotalSalary:
#          maxTotalSalary=s[j].TotalSalary
#          maxIndex=j
#          print("\n Max Salary (Salary+Bonus)")
#          s[maxIndex].PrintManagerInfo()
                  
'''Slip 37: Write a Python script using class to reverse a string word by word.'''

# class String:
#     def get_String(self):
#         self.str=input("Enter a string")
        
#     def reverse(self):
#         str1=self.str[: :-1]
#         print(str1)

# Obj=String()
# Obj.get_String()
# Obj.reverse()        


'''Slip 38: Write a Python class named Student with two attributes student_name, marks. 
Modify the attribute values of the said class and print the original and modified values of the said attributes.'''


'''SLip 39: Program to print Fibonacci series using recursion.'''

# def fibonacci(n):
#     if(n<2):
#         return 1
#     return(fibonacci(n-1)+fibonacci(n-2))

# n=int(input("Enter the number of terms : "))
# for i in range(n):
#     print(fibonacci(i))

'''Slip 40: Write a python program to print the contents of file in reverse order.'''

def program11():
    for i in list(reversed(open("merge.txt","r"))):
        print(i.rstrip())
        print(i)
program11()        



f1=open("merge.txt","r")
f2=f1.read()

reverse=f2[::-1]
print(f2)
print(reverse)


#!/bin/bash #reading data from the user read -p 'Enter a : ' a read -p 'Enter b : ' b  add=$((a + b)) echo Addition of a and b are $add sub=$((a - b)) echo Subtraction of a and b are $sub mul=$((a * b)) echo Multiplication of a and b are $mul div=$((a / b)) echo division of a and b are $div mod=$((a % b)) echo Modulus of a and b are $mod ((++a)) echo Increment operator when applied on "a" results into a = $a ((--b)) echo Decrement operator when applied on "b" results into b = $b    #!/bin/bash #reading data from the user read -p 'Enter a : ' a read -p 'Enter b : ' b if(($a == "true" && $b == "true" )) then 	echo Both are true. else 	echo Both are not true. fi if(($a == "true" || $b == "true" )) then 	echo Atleast one of them is true. else 	echo None of them is true. fi if(( ! $a == "true" )) then 	echo "a" was initially false. else 	echo "a" was initially true. fi    #!/bin/bash #reading data from the user read -p 'Enter a : ' a read -p 'Enter b : ' b  if(( $a==$b )) then 	echo a is equal to b. else 	echo a is not equal to b. fi  if(( $a!=$b )) then 	echo a is not equal to b. else 	echo a is equal to b. fi  if(( $a<$b )) then 	echo a is less than b. else 	echo a is not less than b. fi  if(( $a<=$b )) then 	echo a is less than or equal to b. else 	echo a is not less than or equal to b. fi  if(( $a>$b )) then 	echo a is greater than b. else 	echo a is not greater than b. fi  if(( $a>=$b )) then 	echo a is greater than or equal to b. else 	echo a is not greater than or equal to b. fi   #!/bin/bash #reading data from the user read -p 'Enter file name : ' FileName if [ -e $FileName ] then 	echo File Exist else 	echo File doesnot exist fi if [ -s $FileName ] then 	echo The given file is not empty. else 	echo The given file is empty. fi if [ -r $FileName ] then 	echo The given file has read access. else 	echo The given file does not has read access. fi if [ -w $FileName ] then 	echo The given file has write access. else 	echo The given file does not has write access. fi if [ -x $FileName ] then 	echo The given file has execute access. else 	echo The given file does not has execute access. fi   






    




     


