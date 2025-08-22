a=input("Boy:")
b=input("girl:")
x=list(a)
y=list(b)
for i in range(len(x)):
    for j in range(len(y)):
        if (x[i]==y[i]):
            x[i]=" "
            y[i]=" " 
print(x)
print(y)
c=0
for i in x:
    if(i!=" "):
        c=c+1

for i in y:
    if(i!=" "):
        c=c+1
print(c)
f=0
res=list("flames")
for i in range(5):
    f=((f+(c-1))%len(res))
    res.pop(f)
print(res[0])
