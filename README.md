# hw60: wrap binary search 

### 2: recall inverse functions and logarithms
#### What is meant by y = log2x ?
y = log<sub>2</sub>x is an equation that is the equivalent of saying that 2 raised to the power of y is equal to x.   
      x = 2<sup>y</sup>  
     
#### What does its graph look like?
The graph of this would be located in quadrants I and IV. 
There would be a vertical asymptote at x=0, and have an x-intercept of (1,0).
The graph would have a range of (-∞,+∞) and a domain of (0,+∞).

### 3: describe the recursive solution
#### 0. State the problem
Find the index of `findMe` in an ordered list. 
#### 1. State the recursive abstraction
When this process is asked to return the index of `findMe` in an ordered list, the recursive abstraction can return the index of `findMe` in an ordered list that has half as many elements. 
#### 2. Identify the parts of this solution that correspond to the six parts of a generalized recursive solution.
0. decide between the recursive and base cases  
			base case 0 decision: `if( low > hi)`  
			base case 1 decision: `if( comparison == 0) ` 
1. solution to base case(s)  
			base case 0 solution: `return -2;`  
			base case 1 solution:`return pageToCheck;`
2. solution to recursive case, with these components:  
			a. combiner that combines: N/A  
			b. invocation of the recursive abstraction:  
					`indexOf_recursive( findMe, low, pageToCheck -1);`
					`indexOf_recursive( findMe, pageToCheck -1, hi);`  
			c. leftover processing: N/A  



based on [solutionsHolmes/5F_OrderedList_inArraySlots_v3_Index/](https://github.com/stuyvesant-cs/solutionsHolmes/tree/master/5F_OrderedList_inArraySlots_v3_Index)
as of 2019-04-11 
