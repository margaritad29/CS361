# exercise 5:
found = 0
x = 11
while found < 20:
  if (x % 5 == 0) or (x % 7 == 0) or (x % 11 == 0):
    print (x)
    found += 1
  x +=1


#exercise 6:
#part a:
def is_prime(n):  
  # prime has to be greater than 1
  if n > 1:
    for each in range(2, int(n/2)):
        if(n % each) == 0:
          return False
        break #stop loop from checking forever
    return True
 
    
print(is_prime(13))
print(is_prime(6))
print(is_prime(5))
print(is_prime(22))
  

#part b:
def is_improved_prime(n):
  if n > 1:
    if n == 2 or n == 3:
        return True
    elif (n-1)%6 == 0 or (n+1)%6 == 0:
        if(is_prime(n)):
          return True
        else:
          return False
    else:
      return False

print(is_improved_prime(13))
print(is_improved_prime(6))
print(is_improved_prime(5))
print(is_improved_prime(22))

#part c:
#return all prime up to n
def primes(n):  
  l = []
  # prime has to be greater than 1
  for each in range(n):
    if(is_improved_prime(each)):
      l.append(each)
  
  return l

    
print(primes(10))

#part d:
def get_primes(n):  
  l = []
  if n >= 1:
    #first prime num
    l.append(2)
    i = 2
    x = 3
    while i <= n:
      if(is_improved_prime(x)):
        l.append(x)
        i+=1
      x+=2 #only odds will be prime


  return l

    
print(get_primes(14))

#exercise 7:
#part a:
def print_list(l):
  for each in l:
    print(each)
    
print_list([1,2,3,5])

#part b:
def print_reverse(l):
  for each in l[::-1]:
    print(each)

print_reverse([1,2,3,5])
    
#part c:
def list_length(l):
  length = 0
  for each in l:
    length += 1
  print(length)
  
list_length([1,2,3,5])



#exercise 8:
def set_first_elem_to_zero(l):
  l[0] = 0;
  
set_first_elem_to_zero(a)
print(a)



#exercise 9:
def make_list(l):
  elements = []
  
  for each in l:
    for element in each:
      elements.append(element)
      
  return elements
  
l = [[1,2],[3,4],[5,6,7]]
print(make_list(l))



#exercise 10:
import matplotlib
import matplotlib.pyplot as plt
import numpy as np

# Data for plotting
a = np.arange(0.0, 2.0, 0.01)
b = (np.sin(a - 2) **2) * np.exp(-a **2)

fig, ax = plt.subplots()
ax.plot(a, b)

ax.set(xlabel='x-axis', ylabel='y-axis', title='Function')
#fig.savefig("test.png")
plt.show()



#exercise 11:

#iterative
def mult_list(l):
  result = 1 

  for each in l:
    result *= each
    
  return result

#recursive
def mult_list(l):
	if len(l) == 1:
		return l[0]
	else:
		return mult_list([l[0]])  * mult_list(l[1:])
 
l = [1,2,3,4,5,6]
mult_list(l)


#exercise 12:
def fib(n):
  #f(0)=0 / f(1)=1
  if n == 0 or n == 1:
    return n
  else:
    return fib(n-1) + fib(n-2);
  
fib(10)

exercise 13:
file  = open("emails.txt", "r")

print(re.search('[a-zA-Z]*@[a-zA-Z]*\.[a-zA-Z]*', 'asdfd@asfsd.afs'))

for line in file:
    email = re.search('[a-zA-Z]+@[a-zA-Z]+\.[a-zA-Z]+', line)
    print(email)
