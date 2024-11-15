**Relation**

Let A and B are sets then every possible subset of 'AxB' is called a relation from A to B.

if | A | = m and | B | = n then total no of elements(pair) will be m*n, every element will have two choice weather to present or not present in the subset(relation) therefore the total number of relation possible is 2^mxn

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
