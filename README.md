# Ass-1-9-7-22
Assignment-1
import math
n=51
seive=[]
for i in range(n):
    seive.append(True)
seive[0]=seive[1]=False
x=int(math.sqrt(n))
for i in range(2,x+1):
    if seive[i]:
        for j in range(i*i,n,i):
            seive[j]=False
for i in range(n):
    if seive[i]:
        print(i)
