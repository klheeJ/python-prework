"# python-prework" 
#Question 1
#Write a function to print "hello_USERNAME!" USERNAME is the input of the function. The first line of the code has been defined as below.

def hello_name(user_name):
    """Greet a user"""
    question = input("What is your username? ")
    print("Hello_" + question.upper() + "!")

hello_name(user_name="")



#Question 2 
#Write a python function, first_odds that prints the odd numbers from 1-100 and returns nothing

def first_odds():
    """Prints odds numbers from 1-100"""
    x = 0
    while x < 100:
        x += 1
        if x % 2 == 0:
            continue 
        print(x)

first_odds()




#Question 3
#Please write a Python function, max_num_in_list to return the max number of a given list. The first line of the code has been defined as below.

def max_num_in_list(a_list):
    return max(my_list)

my_list = [34,56,1232,654656]
print(max_num_in_list(a_list=" "))




#Question 4
#Write a function to return if the given year is a leap year. A leap year is divisible by 4, but not divisible by 100, unless it is divisible by 400. 
#The return should be boolean Type (true/false)

def is_leap_year(a_year):
    """Prints whether a year is a leap year or not"""
    a_year = int(input("Is the following year a leap year? "))
    if a_year % 4 == 0 or a_year % 400 == 0:
        a_year = True
    else:
        a_year = False
    return bool(a_year)

print(is_leap_year(a_year=""))




#Question 5
#Write a function to check to see if all numbers in a list are consecutive numbers. For example [2,3,4,5,6,7] are consecutiv e numberss, but [1,2,4,5] are not 
#consecutive numbers. The return should be boolean Type. 

def is_consecutive(a_list):
    sorted_list = sorted(a_list)
    range_list = list(range(min(a_list), max(a_list) +1))
    if sorted_list == range_list:
        return True
    else:
        return False

my_list = [20,21,24,23,22]
print(is_consecutive(my_list))
