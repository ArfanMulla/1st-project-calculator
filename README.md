# 1st-project-calculator

def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiplacatin(a,b):
    return a*b

def division(a,b):
    return a/b


def cal():
    num = int(input("Enter number: "))

    while True:
        op = input("Enter operator (+, -, =): ")

        if op == "=":
            print("Result:", num)
            break

        next_num = int(input("Enter number: "))

        if op == "+":
            num = add(num, next_num)

        elif op == "-":
            num = subtract(num, next_num)

        elif op =="*":
            num = multiplacatin(num,next_num)

        else :
            num = division(num , next_num)

cal()
