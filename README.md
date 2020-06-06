# remove-element-more-than-two-occurance 

#remove element more than two occurance

n=8
l=[10,35,42,10,35,10,68,10] 
ll=[]+l;k=[]
for i in range(n):
    a=l.count(l[i])
    if l.count(l[i])>2 and l[i] not in k:
        k.append(l[i])
        a=a-2
        x=l[i]
        for j in range(n-1,-1,-1):
            if l[i]==l[j]:
                ll.pop(j)
                a-=1
                if a==0:break
print(ll)
        
        
