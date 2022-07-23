# Prototype_3
def fact(n):        
    f = 1
    for i in range(n, 1, -1):
        f *= i
    return f

stroka = ''    
k = 0
for i in range(60000, 1000, -1):
    s = str(i)
    if int(max(s))**2 >= fact(int(max(s)) - int(min(s))):
        k += 1
        stroka += s
        if k == 15:
            break
        
a = [0] * (int(max(stroka))+1)  
for j in range(len(stroka)):
    n = int(stroka[j])
    a[n] += 1
    
i = a.index(max(a))
print(i)
