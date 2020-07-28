n=input()
k = [0 for i in range(100)]
cnt=0
def isPrime(a):
  if(a<2):
    return False
  for i in range(2,a):
    if(a%i==0):
      return 
  return int(a)

for i in range(int(n)+1):
    if(isPrime(i)):
        k[cnt] = isPrime(i)
        cnt= cnt+1
for i in range(100):
    for j in range(i):
        if n == k[i] + k[j]:
            print(k[i],k[j])
# 아직 완성되지 않았음
# 소수를 넣는 배열인 k는 잘 구현되지만 출력이 않됨
