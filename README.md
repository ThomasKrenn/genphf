# Generating Perfect Hash Functions

## Algorithm Overview

1. Start with a square table that is t units on a side.
2. Place each key K in the table at location (row,col), where row=K/t, col=K mod t.
3. Collapse the table down into a linear array and create a row displacment table; this is our hash table.
4. The hash function uses t and the displacements from step 3 to locate K.

[Perfect Hashing Using Sparse Matrix Packing](https://people.engr.ncsu.edu/tharp/Infosys/Course_2010/sparse_matrix_packing.pdf)

[Bin Packing Problem](https://en.wikipedia.org/wiki/Bin_packing_problem) Bin Packing Problem

[Bin Packing German](https://algo.rwth-aachen.de/~algorithmus/algo24.php) Bin Packing

To be continued.
