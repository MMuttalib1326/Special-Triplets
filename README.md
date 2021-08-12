# Special-Triplets
Gintoki has been very lazy recently and he hasn't made enough money to pay the rent this month. So the old landlady has given him a problem to solve instead, if he can solve this problem the rent will be waived. The problem is as follows:  A triplet of integers (A,B,C) is considered to be special if it satisfies the following properties for a given integer N :  AmodB=C BmodC=0 1≤A,B,C≤N


for _ in range (int(input())):
    n=int(input())
    MM=0
    for i in range(1,n+1):
        for j in range(i,n+1,i):
            if(j%i==0):
                for k in range(i,n+1,j):
                    if(k%j==i):
                        MM+=1
    print(MM)      
