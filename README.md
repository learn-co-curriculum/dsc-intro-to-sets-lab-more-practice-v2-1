
# Introduction to Sets - More Practice - Lab

## Introduction

In previous sections in this Module, you learned about sets, defining sets and performing set operations in Python, and how to visualize set operations using Venn Diagrams. 

In the Appendix to this Module, we included a lesson to teach you more about set notation, and about the inclusion/exclusion principle. In this Appendix lab, you will have an opportunity to solve some problems regarding set operations using Venn diagrams, as well as solve problems using Python involving the inclusion/exclusion principle. 

## Objectives

You will be able to:

* Use Venn diagrams to visually demonstrate set operations
* Use Python to perform set operations
* Use Python to demonstrate the inclusion/exclusion principle

## Exploring Set Operations Using a Venn Diagram

Let's start with a pretty conceptual example. Let's consider the following sets:

   - $\Omega$ = positive integers between [1, 12]
   - $A$= even numbers between [1, 10]
   - $B = \{3,8,11,12\}$
   - $C = \{2,3,6,8,9,11\}$
    

#### a. Illustrate all the sets in a Venn Diagram like the one below. The rectangular shape represents the universal set.

<img src="./images/venn_diagr.png" width="600">


#### b. Using your Venn Diagram, list the elements in each of the following sets:

- $ A \cap B$
- $ A \cup C$
- $A^c$ 
- The absolute complement of B
- $(A \cup B)^c$
- $B \cap C'$
- $A\backslash B$
- $C \backslash (B \backslash A)$ 
- $(C \cap A) \cup (C \backslash B)$

## The Inclusion Exclusion Principle

Use A, B and C from the previous exercise to verify the inclusion exclusion principle in Python.

Recall from the lesson in the Appendix that:

$$\mid A \cup B\cup C\mid = \mid A \mid + \mid B \mid + \mid C \mid - \mid A \cap B \mid  -\mid A \cap C \mid - \mid B \cap C \mid  + \mid A \cap B \cap C \mid $$

Combining these main commands:

| Method        |	Equivalent |	Result |
| ------                    | ------       | ------    |
| a.union(b)                |	A $\mid$ B | new set with elements from both a and b
| a.intersection(b)         |	A & B      | new set with elements common to a and b

along with the `len(x)` function to get to the cardinality of a given x ("|x|").

What you'll do is translate the left hand side of the equation for the inclusion principle in the object `left_hand_eq`, and the right hand side in the object `right_hand_eq` and see if the results are the same.



```python
left_hand_eq = None
print(left_hand_eq)  # 9 elements in the set
```


```python
right_hand_eq = None
print(right_hand_eq) # 9 elements in the set
```


```python
None # Use a comparison operator to compare `left_hand_eq` and `right_hand_eq`. Needs to say "True".
```

## Summary

In this lab, you practiced your knowledge on sets, such as common set operations, the use of Venn Diagrams, the inclusion exclusion principle, and how to use sets in Python! 
