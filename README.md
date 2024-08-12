# kadenes-algorithem-max-number-
def maxSubArraySum(a):
  current=a[0]
  total=a[0]
  for i in range(1,len(a)):
    current=max(a[i],current+a[i])
    total = max(total,current)
  return total
my_list=[-2,-3,4,-1,-2,1,5,-3]
print(maxSubArraySum(my_list))
