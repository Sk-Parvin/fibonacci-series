# fibonacci-series
n = int(input("Enter the number of terms in the Fibonacci series: "))
firstTerm = 0
secondTerm = 1
print("Fibonacci series:", firstTerm, secondTerm, end=" ")
for i in range(3, n+1):
    nextTerm = firstTerm + secondTerm
    print(nextTerm, end=" ")
    firstTerm = secondTerm
    secondTerm = nextTerm
