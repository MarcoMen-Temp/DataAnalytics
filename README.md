# DataAnalytics
 Ian McLoughlin
# A program that displays Fibonacci numbers using people's names.
#
"""Hi Ian

My surname is Men. Coincidentally,the 1st and last letters are identical to your surname "M" and "n",which the sum would give the same result as the file we copied and paste. For this reason, I decided to use the letters of my first name "Marco" and I tried with my 2nd name " Filipe"



After googling (perhaps not a proper verb) " ord () ",which lead me to sites such as GeeksforGeek.org and stackoverflow. The definition is the inverse of Chr() -Return the Unicode code point for one character string . Example: on my first name ,the first letter is an " M " with an Unicode number of 77; and the last letter " o " with the value of 111. The sum of the 2 is 188 ( fib1.py )

My second name  " Filipe ", the same principle applies . Unicode values for :

- " F " is 70 and " e " is 101. The sum of both is 171 ( fib2.py )

I used the following site https://unicode-table.com/en/#004D , to confirm the values ( defined as HTML - code )



Regards 



Marco"""


def fib(n):
  """This function returns the nth Fibonacci number."""
  i = 0
  j = 1
  n = n - 1

  while n >= 0:
    i, j = j, i + j
    n = n - 1
  
  return i

name = "Filipe"
first = name[0]
last = name[-1]
firstno = ord(first)
lastno = ord(last)
x = firstno + lastno

ans = fib(x)
print("My surname is", name)
print("The first letter", first, "is number", firstno)
print("The last letter", last, "is number", lastno)
print("Fibonacci number", x, "is", ans)
