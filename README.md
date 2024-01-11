# data-structure
#sorting techinque
#Bubble sort:

n=int(input("enter no of elements:"))
A=[]
for i in range(n):
    a=int(input("enter list element  :"))
    A.append(a)
print("list A contain =",A)

def bubble():
    for i in range(n):
        flag=0
        for j in range(0,n-i-1):
              if A[j]>A[j+1]:
                    b=A[j]
                    A[j]=A[j+1]
                    A[j+1]=b
                    flag=1
        if flag==0:
             break
bubble()                                                                                                                    
print("Sorted list by bubble sort=",A)


#selection sort:

index=0
for i in range (n-1):
    min=A[i]
    minindex=1
    for j in range(i+1, n):
        if min>A[j]:
           min=A[j]
           minindex=j
           A[i],A[minindex]=A[minindex],A[i]         
print("Sorted List by selection sort=",A)


