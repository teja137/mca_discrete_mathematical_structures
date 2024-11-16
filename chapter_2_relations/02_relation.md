**Relation**

Let A and B are sets then every possible subset of 'AxB' is called a relation from A to B.

if | A | = m and | B | = n then total no of elements(pair) will be m*n, every element will have two choice weather to present or not present in the subset(relation) therefore the total number of relation possible is 2^m*n

e.g.:

    A = {a,b}
    B = {1,2,3}
    R = {(a,1),(a,3),(b,2)}

    ![alt text](image-1.png)

e.g.:

    A = {a,b}
    B = {1,2}
    AxB = {(a,1),(a,2),(b,1),(b,2)} - total number of elements
    total number of relation possible is 2^mxn -> 2^ 2*4

(a,1), (a,2), (b,1), (b,2), Total Possible Relations
----------------------------------------------------
0      , 0      , 0      , 0      , {}
1      , 0      , 0      , 0      , {(a,1)}
0      , 1      , 0      , 0      , {(a,2)}
0      , 0      , 1      , 0      , {(b,1)}
0      , 0      , 0      , 1      , {(b,2)}
1      , 1      , 0      , 0      , {(a,1), (a,2)}
1      , 0      , 1      , 0      , {(a,1), (b,1)}
1      , 0      , 0      , 1      , {(a,1), (b,2)}
0      , 1      , 1      , 0      , {(a,2), (b,1)}
0      , 1      , 0      , 1      , {(a,2), (b,2)}
0      , 0      , 1      , 1      , {(b,1), (b,2)}
1      , 1      , 1      , 0      , {(a,1), (a,2), (b,1)}
1      , 1      , 0      , 1      , {(a,1), (a,2), (b,2)}
1      , 0      , 1      , 1      , {(a,1), (b,1), (b,2)}
0      , 1      , 1      , 1      , {(a,2), (b,1), (b,2)}
1      , 1      , 1      , 1      , {(a,1), (a,2), (b,1), (b,2)}


**Complement of a relation**

Let R be a relation from A to B, then the complement of relation will be denoted by R', R^C, or 𝑅.

R' = {(a,b)|(a,b) ∈ AxB, (a,b) ∈! R}
R' = (AxB) - R
Relation complement = Universal set - Relation

e.g.:

    if AxB = {(a,1),(a,2),(a,3),(b,1),(b,2),(b,3)} // Cartesian product
    R (Relation) = {(a,1),(a,3),(b,2)} // suppose take 3 elements from above. The left overs are called complement.

    U (Universe) = AxB  
    R' (Relation complement) =  {(a,2),(b,1),(b,3)}

e.g.:

    R U R' = AxB
    R n R' = ∅

**Inverse of a relation**

Let R be a relation from A to B, then the inverse of relation  will be a relation from B to A, denoted by R^-1.

R^-1 = {(b,a) | (a,b) b ∈ R}

AxB = {(a,1), (a,2), (a,3), (b,1), (b,2), (b,3)}
R = {(a,1),(a,3),(b,2)}
R^-1 = {(1,a),(3,a),(2,b)}

|R| == |R^-1|

**Diagonal relation:**

A relation R on a set A is said to be diagonal relation if, R is a set of all ordered pair (x,x), for every ∀x ∈ A, sometime it is also denoted by 
Δ 
 A

R = {(x,x) | ∀ x ∈ A }

e.g.:

    A = {1,2,3}
    AxA = {(1,1),(2,2),(3,3)}

        1   2   3
    1   11
    2       22
    3           33


**Types of a Relation**

To further study types of relation, we consider a set A with n elements, then  a cartesian product AxA will have n^2 elements(pairs).
Therefore, total number of relations possible is 2^n*n

**Reflexive relation**

A relation R on a set A is said to be reflexive, 
if, ∀ x ∈ A
    (x,x) ∈ A

        1   2   3
    1   11
    2       22
    3           33

    e.g.:

    A = {1,2}
    AxA = {(1,1),(1,2),(2,1),(2,2)}
    here it is reflexive because it contains (1,1) and (2,2)

**Irrelative relation**

A relation R on a set A is said to be Irrelative,
if ∀ x ∈ A
    (x,x) ∉ A

**difference between Reflexive and Irrelative relation:**

no  Relation                        Reflexive   -   Irrelative
1   AxA                                 ✓              ✘
2   ∅                                   ✘              ✓ 
3   {(1,1),(2,2),(3,3)}                 ✓              ✘
4   {(1,2),(2,3),(1,3)}                 ✘              ✓
5   {(1,1),(1,2),(2,1),(2,2)}           ✘              ✘
6   {(1,1),(2,2),(3,3),(1,3),(2,1)}     ✓              ✘
7   {(1,3),(2,1),(2,3),(3,2)}           ✘              ✓


E.g.:

if A = {a,b}, AxA = {(a,a),(a,b),(b,a),(b,b)}

| (a, a) | (a, b) | (b, a) | (b, b) | Relation Subset                     | Reflexive | Irrelative |
|--------|--------|--------|--------|-------------------------------------|-----------|-------------|
|   0    |   0    |   0    |   0    | {}                                  | No        | Yes         |
|   1    |   0    |   0    |   0    | {(a, a)}                            | No        | No          |
|   0    |   1    |   0    |   0    | {(a, b)}                            | No        | Yes         |
|   0    |   0    |   1    |   0    | {(b, a)}                            | No        | Yes         |
|   0    |   0    |   0    |   1    | {(b, b)}                            | No        | No          |
|   1    |   1    |   0    |   0    | {(a, a), (a, b)}                    | No        | No          |
|   1    |   0    |   1    |   0    | {(a, a), (b, a)}                    | No        | No          |
|   1    |   0    |   0    |   1    | {(a, a), (b, b)}                    | Yes       | No          |
|   0    |   1    |   1    |   0    | {(a, b), (b, a)}                    | No        | Yes         |
|   0    |   1    |   0    |   1    | {(a, b), (b, b)}                    | No        | No          |
|   0    |   0    |   1    |   1    | {(b, a), (b, b)}                    | No        | No          |
|   1    |   1    |   1    |   0    | {(a, a), (a, b), (b, a)}            | No        | No          |
|   1    |   1    |   0    |   1    | {(a, a), (a, b), (b, b)}            | Yes       | No          |
|   1    |   0    |   1    |   1    | {(a, a), (b, a), (b, b)}            | Yes       | No          |
|   0    |   1    |   1    |   1    | {(a, b), (b, a), (b, b)}            | No        | No          |
|   1    |   1    |   1    |   1    | {(a, a), (a, b), (b, a), (b, b)}    | Yes       | No          |


**Symmetric relation**

A relation R on a set A is said to be symmetric,
if  ∀ a,b ∈ A
    (a,b) ∈ A
then (b,a) ∈ R

**Equivalence relation**

A relation R on a set A with cartesian product AxA is said to be Equivalence, if it is

1. Reflexive // If A = {1,2,3}, then reflexive is (1,1)(2,2)(3,3)
2. Symmetric // if R is (1,2) then symmetric is R = {(1,2),(2,1)}
3. Transitive // if R is (1,2) and R is (1,3) then Transitive relation is (1,3)

If two relations R1 and R2 are equivalence then their union need not to be equivalence but intersection will also br Equivalence.

R1: (a,b) iff(if and only if) (a+b) is even over the set of integers.

**Partial order relation**

A relation R ona set A with cartesian product AxA is said to be partial order, if it is

1. Reflexive
2. Anti - Symmetric
3. Transitive

**Partial ordering ser (Poset)**

A set A with partial ordering relation R defined on A is called a POSET and is denoted by [A,R]

e.g.:

    [A,/], [A,<=],[P(S),⊆]

    e.g.:
    {1,2,3} <=
    if a<= b
        (a,b) ∈ R

    {(1,1),(1,2),(1,3)
            (2,2),(2,3)
                 ,(3,3)}