# Multiobjective Set Covering Problems (SCP)


## Definition	
The set covering problem with two objectives is defined as follow:

    Min sum{j=1,…,n} c1(j) x(j)
    Min sum{j=1,…,n} c2(j) x(j)
    s/t sum{j=1,…,n} t(i,j) x(j) >= 1   for i=1,…,m
         x(j) = 0 or 1                  for j=1,…,n


## Description
There are currently 44 data files.

They correspond to 11 bi-objective set covering problems.

For each problem, 4 variants are given: class A, B, C and D:

+ A: the costs are uniformly generated
+ B: created from A by replacing the second vector of costs by the first one in reverse order
+ C: vector of costs generated with plateaus of values
+ D: created from C by replacing the second vector of costs by the first one in reverse order


## Format
The format is originally from the OR library extended for handling multiple objectives.

The format of all of these data files is:

    number of rows (m), number of columns (n)   
    the cost of each column for objective 1 c1(j),j=1,...,n
    the cost of each column for objective 2 c2(j),j=1,...,n 
    for each row i (i=1,...,m): the number of columns which cover row i followed by a list of the columns which cover row i


## Files
Link to data files.


## Misc
Files contain data from
> Xavier Gandibleux, David Vancoppenolle and Daniel Tuyttens.
 A first making use of GRASP for solving MOCO problems
 14th International Conference in Multiple Criteria Decision-Making
 June 8–12, 1998, Charlottesville, USA.