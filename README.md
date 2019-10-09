n = int(input())
if n >= 5 and n % 2 != 0:
    arr = []
    for j in range(1, n+1):
        if j % 2 != 0:
            arr.append(j)
    k = arr.index(n) + 1
    for a in range(k):
        star0 = " "*(k-1-a) + "*"*(2*a+1)
        print(star0)
    for b in range(k):
        star1 = "@" + " "*(n-2)+ "@"
        print(star1)
    for c in range(k):
        if c != k-1:
            star2 = "@" + " "*(k-2-c) + "*"*(2*c+1) + " "*(k-2-c) + "@"
        else:
            star2 = "*"*(2*c+1)
        print(star2)
else:
    print("Enter the odd integer 5 or greater")
