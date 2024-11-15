**Operations on sets**

**Complement of set**
The complement of a set refers to the elements that are not in the set, but belong to a universal set 
𝑈
U that contains all the possible elements under consideration.
(A complement C) A^c = { x | x ∉ A & x ∈ U }

e.g.:
    U = {1,2,3,4,5,6}
    A = {2,3,6}
    A^c = {1,4,5}


A U A^c = U
A n A^c = ∅
U^c = ∅
∅^c = U

**Union of sets**

Union of two sets A and B is a set of all those elements which either belong to A or B or both, it is denoted by A U B

A U B =  {x | x ∈ A or x ∈ B }

e.g.:

    A = {1,2,3,4}
    B = {3,4,5,6}
    A U B = {1,2,3,4,5,6}


question:

is
| A | + | B | = | A U B | ??????
  4   +   4   =  6 - its wrong

  the real formula is:

  |A U B| = | A | + | B | - |A n B|

**Intersection set**

Intersection of two sets A and B is a set of all those elements which belong to both A and B, and is scented by A n B.

A n B = { x | x ∈ A and x ∈ B }


e.g.:

    A = {1,2,3,4}
    B = {3,4,5,6}

    A n B = {3,4}


**Disjoints sets**

Two sets are said to be disjoint if they do not have a common element, i.e. no elements in A is in B and no elements in B is in A.

A n B = ∅

**Set Difference**

The set difference of two sets A and B, is the set of all the elements which belongs to A but do not belong to B.

A - B = { x | x ∈ A and x ∉ B }
it can also be written as
A \ B = { x | x ∈ A and x ∉ B }

e.g.:

    A = {1,2,3,4}
    B = {3,4,5,6}
    A - B = {1,2}
    B \ A = {3,4}

A U B = B U A
A n B = B n A
A - B != B - A
A \ B != B \ A

**Symmetric difference**

The symmetric difference of two sets A and B is the set of all the elements that are in A or in B but not in both, denoted as A ⊕ B = ( A u B) - (A n B)

A ⊕ B = { x | x ∈ A and x ∉ B } or (x ∈ B and x ∉ A)

note:
'or' means u
'and' means n

A ⊕ B = (A - B) u (B - A)

A = {1,2,3,4}
B = {3,4,5,6}

A ⊕ B = {1,2,5,6}