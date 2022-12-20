# day-5
decode 111-aaa,ka,ak

a=(input())
b=len(a)
m=1
n=2
if a[0]!=0:
    if len(a)==1:
        print(m)
    elif len(a)==2:
        print(n)
    else:
        for i in range(1,b-1):
            c=int(m)+int(n)
            m=n
            n=c
        print(c)
