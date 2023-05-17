# Programming_Assingment-4

1. Write a Python Program to Find the Factorial of a Number?
Sol.
num = int(input("Enter a number: "))

fact = 1
for i in range(num, 0, -1):
    fact = fact*i
    
print("\nFactorial of {}: {}".format(num, fact))
o/p:
Enter a number: 5

Factorial of 5: 120



2. Write a Python Program to Display the multiplication Table?
Sol.
num = int(input("Enter a number: "))

for i in range(1, 11):
    print("{} x {} = {}".format(num, i, num*i))
o/p:
Enter a number: 4
4 x 1 = 4
4 x 2 = 8
4 x 3 = 12
4 x 4 = 16
4 x 5 = 20
4 x 6 = 24
4 x 7 = 28
4 x 8 = 32
4 x 9 = 36
4 x 10 = 40




3. Write a Python Program to Print the Fibonacci sequence?
Sol.
fibo_length = int(input("Enter a length: "))

a = 0
b = 1
print(a, end = ' ')
print(b, end = ' ')
while(fibo_length-2 > 0):
    nt = a + b
    print(nt, end = ' ')
    a = b
    b = nt
    
    fibo_length -= 1
o/p:
Enter a length: 11
0 1 1 2 3 5 8 13 21 34 55



4. Write a Python Program to Check Armstrong Number?
Sol.
import math
def fibo_check(num):
    l = len(str(num))  ## l = number of digits of number
    sum1 = 0 
    temp_num = num
    while(num > 0):
        d = num % 10
        sum1 += int(math.pow(d, l))
        num = num // 10

    if(sum1 == int(temp_num)):
        return 1
    else:
        return 0
num = int(input("Enter a number: "))

if(fibo_check(num)):
    print("{} is an armstrong number".format(num))
else:
    print("{} is not an armstrong number".format(num))
Enter a number: 153
153 is an armstrong number
num = int(input("Enter a number: "))

if(fibo_check(num)):
    print("{} is an armstrong number".format(num))
else:
    print("{} is not an armstrong number".format(num))
Enter a number: 1221
1221 is not an armstrong number



5. Write a Python Program to Find Armstrong Number in an Interval?
Sol.
low = int(input("Enter the lower value of range: "))
high = int(input("Enter the higher value of range: "))

print("\nFrom {} to {} following are the Armstrong Number:".format(low, high), end='\n')
for i in range(low, high+1):
    
    if(fibo_check(i)):
        print(i, end = ' ')
Enter the lower value of range: 100
Enter the higher value of range: 1500

From 100 to 1500 following are the Armstrong Number:
153 370 371 407



6. Write a Python Program to Find the Sum of Natural Numbers?
Sol.
num = int(input("Enter a positive number: "))

total_sum = 0
for i in range(1, num+1):
    total_sum += i
    
print("Sum of {} natural number is {}".format(num, total_sum))
Enter a positive number: 100
Sum of 100 natural number is 5050


