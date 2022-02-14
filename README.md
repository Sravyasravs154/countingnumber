# Count = 0
def Counting(Number):
    global Count
    if(Number > 0):
        Count = Count + 1
        Counting(Number//10)
    return Count

Number = int(input("Please Enter any Number: "))
Count = Counting(Number)
print("\n Number of Digits in a Given Number = %d" %Count)
