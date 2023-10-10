# febonacci.py
# fibonacci series#function def
def fibonacci(n):
    first=[0,1]
    for i in range(2,n):
        next=first[-1]+first[-2]
        first.append(next)
    return first
n=int(input("enter the number pf terms for the fibonacci series:"))
if n<=0:
    print("plese enetr a positive integer")
else:
    fibonacci_series=fibonacci(n)
    print("fibonacci_series:")
    for term in fibonacci_series:
        print(term,end=" ")

