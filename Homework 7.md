
# Part 1
### A
- I would choose quick sort to do the first list, as it has an average time complexity of O(nlogn), and it has a good average time conplexity. It does not need the same memory that merge sort needs, and it still retains the average time complexity of nlogn
## B
- I would choose heapsort for this sorting algorithm, as it retains the nlogn comparisons for all cases, while using less memory due to it being an in place algorithm
## C
- I would choose merge sort then, as it performs close to linear time in that case when the elements are almost sorted
## D
- For short list with large elements, I am again going to choose insertion sort, as it is an in place algorithm, good for those large elements, and it performs relatively well on short lists

# Part 2
To be honest I am not very sure on what this algorithm is. I know that it is taking the keys from the list, and looking for one of them, so that makes sense, it just is confusing on how to implement. I have done by best below.
**Major Factors**:
- Making sure that you have enough memory to load the item when you find it
- Making sure to only load the keys, and not the whole list until you have the item that you are looking for.
**Pseudo Code Below**
```
keys = load keys
target = target key
for key in list:
	if key == target
	load item into memory
	return item to be used
```
- According to the linked text, actions done in memory are free, so this would have a time complexity of o(n), as we are going through n keys, and then loading it into memory and returning it.
# Part Three
### Problems where we have them in polynomial time
- Sorting everyone on the planet by their wealth. We can use a sorting algorithm to do this, while it may be a large number, its a finite amount of people, and we can use a sorting algorithm(Made this one up)
- Finding the highest scoring school in the state. Simpler to the above problem, we can solve this in the time complexity of n, or even faster if the list is sorted.(Made this one up)
### Problems we have proven to be intractable
- Factoring a number into primes in an example of a problem that we know is intractable, we use it for the basis of encryption in many cases, as there is no way to solve it efficiently(https://www.umsl.edu/~siegelj/information_theory/classassignments/Lombardo/04_intractableproblems.html)
- The SAT problem, where you need to find if you can prove a specific formula. This grows exponentially, thus there is no way to solve it in polynomial time.(https://www.umsl.edu/~siegelj/information_theory/classassignments/Lombardo/04_intractableproblems.html)
### Problems not proven either way
- Surprisingly, the TSP problem is one of the ones that we have not proven to be either intractable, or solvable in polynomial time. You have to find the shortest route between all of the cities, and return to the start.(https://crystal.uta.edu/~kumar/CSE5311_09FLDAA/DOCS/module11.pdf)
- Another one, is the graph coloring problem. Same as the above one, we have not been able to prove it either way. In this problem, you have to to find the minimum number of colors that you would be able to color a graph with, without any of the nodes near each other being the same color (https://crystal.uta.edu/~kumar/CSE5311_09FLDAA/DOCS/module11.pdf)
# Part 4
**Pseudo Code**
```
L = Solved List
W = Matrix
Visted = []
flag = true

For verticie in L
	if l can connect to l+1 according to W:
		do nothing
	else:
		return false
return true at the end

```

# Part 5
```
def addtolist(n):
	p = index of processors
	steps = n/p
	list = []
	for n in range(steps):
		give processor p n/steps numbers
		add to list [last operation, n]
	# wait for processors to finish
	return list

```