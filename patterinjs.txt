# Pattern #1: Simple Number Triangle Pattern
# Pattern:
# 1  
# 2 2  
# 3 3 3  
# 4 4 4 4  

numbOfRows = 4
for m in range(1, numbOfRows+1):
    for n in range(1, m+1):
        print(m, end=' ')
    print()



# Pattern #2: Inverted Pyramid of Numbers
# Pattern:
# 1 1 1 1 1 
# 2 2 2 2 
# 3 3 3 
# 4 4 
# 5

numbOfRows = 5
for m in range(1, numbOfRows+1):
    for n in range(numbOfRows, m-1,-1):
        print(m, end=' ')
    print()



# Pattern #3: Half Pyramid Pattern of Numbers
# Pattern:
# 1 
# 1 2 
# 1 2 3 
# 1 2 3 4 
# 1 2 3 4 5


numbOfRows = 5
for m in range(1, numbOfRows+1):
    for n in range(1, m+1):
        print(n, end=' ')
    print()

# Pattern #4: Inverted Pyramid of Descending Numbers
# Pattern:
# 5 5 5 5 5 
# 4 4 4 4 
# 3 3 3 
# 2 2 
# 1

rows = 5
for i in range(rows, 0, -1):  
    num = i  
    for j in range(0, i):  
            print(num, end=" ")       
    print()  

# Pattern #5: Inverted Pyramid of the Same Digit
# Pattern:
# 5 5 5 5 5 
# 5 5 5 5 
# 5 5 5 
# 5 5 
# 5

r=5
for i in range(r+1,0,-1):
    for j in range(0,i-1):
        print("5 ",end="")
    print()        


# Pattern #6: Reverse Pyramid of Numbers
# Pattern:
# 1 
# 2 1 
# 3 2 1 
# 4 3 2 1 
# 5 4 3 2 1

last_num = 6
for row in range(1, last_num):
    for column in range(row, 0, -1):
        print(column, end=' ')
    print("")

# Pattern #7: Inverted Half Pyramid Number Pattern
# Pattern:
# 0 1 2 3 4 5 
# 0 1 2 3 4 
# 0 1 2 3 
# 0 1 2 
# 0 1
 
rows = 5
for i in range(rows,0,-1):   
        for j in range(0, i + 1):  
            print(j, end=" ")       
        print()  

# Pattern #8: Pyramid of Natural Numbers Less Than 10
# Pattern:
# 1 
# 2 3 4 
# 5 6 7 8 9

rows = 3  
num = 1
stop = 2
 
for i in range(rows):  
        for j in range(1, stop):  
            print(num, end=" ")     
            num += 1  
        print() 
        stop += 2 
   
# Pattern #9: Reverse Pattern of Digits from 10 
# Pattern:
# 1
# 3 2
# 6 5 4
# 10 9 8 7

stop = 2
start = 1

current_num = stop
for row in range(2, 6):
    for col in range(start, stop):
        current_num -= 1
        print (current_num, end=' ')
    print("")
    start = stop
    stop +=row
    current_num = stop
 
 
 
# Pattern #10: Unique Pyramid Pattern of Digits
# Pattern:
# 1 
# 1 2 1 
# 1 2 3 2 1 
# 1 2 3 4 3 2 1 
# 1 2 3 4 5 4 3 2 1
 
rows = 6
for i in range(1, rows+1):  
        for j in range(1, i-1):  
            print(j, end=" ")     
            num += 1  
        for j in range(i-1,0,-1):  
            print(j, end=" ")     
             
        print()     

# Pattern #11: Connected Inverted Pyramid Pattern of Numbers
# Pattern:
# 5 4 3 2 1 1 2 3 4 5 
# 5 4 3 2 2 3 4 5 
# 5 4 3 3 4 5 
# 5 4 4 5 
# 5 5

r=6
for i in range(0,r):
    for j in range(r-1,i,-1):
        print(j,"",end=" ")
    for k in range (i):
        print("",end="")
    for l in range(i+1,r):
        print(l,"",end="")
    print("\n")

# Pattern #12: Even Number Pyramid Pattern
# Pattern:
# 10 
# 10 8 
# 10 8 6 
# 10 8 6 4 
# 10 8 6 4 2

rows = 5
lastnum = 2 * rows
even = lastnum
for i in range(1, rows+1):  
  even = lastnum
  for j in range(i): 
    print(even, end=" ")     
    even -= 2  
  print()            
 
# Pattern #13: Pyramid of Horizontal Tables
# Pattern:
# 0  
# 0 1  
# 0 2 4  
# 0 3 6 9  
# 0 4 8 12 16  
# 0 5 10 15 20 25  
# 0 6 12 18 24 30 36

rows = 7
for i in range(0, rows):  
    for j in range(0, i+1):  
      print(i*j, end=" ")            
    print()         

# Pattern #14: Pyramid Pattern of Alternate Numbers
# Pattern:
# 1 
# 3 3 
# 5 5 5 
# 7 7 7 7 
# 9 9 9 9 9

rows = 5  
i = 1
while i <= rows:
    j = 1
    while j <= i:
        print((i * 2-1), end=" ")
        j += 1
    i +=  1
    print()

# Pattern #15: Mirrored Pyramid (Right-angled Triangle) Pattern of Numbers
# Pattern:
#            1 
#          1 2 
#       1 2 3 
#    1 2 3 4 
#  1 2 3 4 5
 
rows = 6
for i in range(1, rows):
    num = 1
    for j in range(rows, 0, -1):
        if j > i:
            print(" ", end=' ')
        else:
            print(num, end=' ')
            num += 1
    print("") 

# Pattern #16: Equilateral Triangle with Stars (Asterisk Symbol)
# Pattern:
#             *   
#            * *   
#           * * *   
#          * * * *   
#         * * * * *   
#        * * * * * *   
#       * * * * * * *
 
n=20
for i in range(1, 8):
    print(' '*n, end='') # repet space for n times
    print('* '*(i)) # repeat stars for i times
    n-=1 

# Pattern #17: Downward Triangle Pattern of Stars
# Pattern:
#         * * * * * * 
#          * * * * * 
#           * * * * 
#            * * * 
#             * * 
#              * 

rows = 6  
m = (2*rows)-2
for i in range(rows-1,-1,-1):  
        for j in range(m,0,-1):  
            print(end=" ")
        m += 1 
        for j in range(0, i+1):  
            print("*",end=" ")               
        print()  
 
 
 
#    Pattern #18: Pyramid Pattern of Stars
# Pattern:
# * 
# * * 
# * * * 
# * * * * 
# * * * * *
for i in range(0,5):
    for j in range(0,i+1):
        print("* ",end="")
    print()        


# a = 8
# for i in range(0, 5):
#     for j in range(0, a):
#         print(end=" ")
#     a = a - 2
#     for j in range(0, i+1):
#         print("* ", end="")
#     print()