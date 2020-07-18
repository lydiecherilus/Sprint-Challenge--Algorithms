#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) Linear O(n) - increase linear with input
    a = 0 - runs one time 
    while (a < n * n * n): run n times
        a = a + n * n run one time

b) Quadratic Complexity (O(n^2)) - nested loops
    sum = 0
    for i in range(n): O(n)
      j = 1
      while j < n: O(n)
        j *= 2
        sum += 1

c) Linear O(n) - being called recursively n times before reaching base case
    def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)


## Exercise II
Use a Binary Search Tree -- Θ(log(n))
1) find the middle floor
    middle_floor = number_of_floors // 2
2) if the egg drops at the the middle floor breaks. we eliminate all the higher floors and set a new middle floor
    middle_floor = middle_floor // 2
3) if the egg drops at the the middle floor does not break. we eliminate all the lower floors and set a new middle floor
    middle_floor = middle_floor + middle_floor // 2

4) start the process again

