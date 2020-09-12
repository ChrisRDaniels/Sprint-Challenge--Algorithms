#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)  a = 0
    while (a < n * n * n):
      a = a + n * n
      
answer: Linear O(n), The first line will only run once O(1). The amount of times
the loop will run depends on n.

b)  sum = 0
    for i in range(n):
      j = 1
      while j < n:
        j *= 2
        sum += 1
        
answer: Linearithmic O(n log n), The first loop is O(n). The second loop is O(log n)

c)  def bunnyEars(bunnies):
      if bunnies == 0:
        return 0
        
answer: O(n), first two lines O(1) only run a set amount of times regardless of input size. 
Last line is O(n) that starts a loop that runs in scale with n.

## Exercise II

I would divide the number of floors in half, and drop the egg from that mid point. If the egg broke, I would divide 
the lower half again. If it did not break, I would divide the higher half. I would continue this until I no longer 
had multiple floors, which  should narrow down the list of floors to the breaking point of the egg.
I believe the complexity would be O(n log n) because it's similar to a merge_sort.
