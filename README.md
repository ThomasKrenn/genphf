# Generating Perfect Hash Functions

## Algorithm Overview

1. Start with a square table that is t units on a side.
2. Place each key K in the table at location (row,col), where row=K/t, col=K mod t.
3. Collapse the table down into a 1D array and a row displacement array; this is our hash table.
4. The hash function H uses t and the displacements from step 3 to locate K.

The hash function is 

  row = K/t<br>
  col = K mod t<br>
  index for 1D array = displacement[row]+col<br>
  H(K) = 1D[index]<br>

Collapsing the table is a bin packing problem. The first-fit decreasing method does result in acceptable table compression. The algorithm can be implemented to have a running time of at most O(n\log(n))

[Perfect Hashing Using Sparse Matrix Packing](https://people.engr.ncsu.edu/tharp/Infosys/Course_2010/sparse_matrix_packing.pdf)

[Bin Packing Problem](https://en.wikipedia.org/wiki/Bin_packing_problem) Bin Packing Problem

[Bin Packing German](https://algo.rwth-aachen.de/~algorithmus/algo24.php) Bin Packing

[Modern perfect hashing for strings](http://0x80.pl/notesen/2023-04-30-lookup-in-strings.html) - Modern perfect hashing for strings


