Author:     Andrius Kelly
Assignment: CS 344 Project 1
Description: Bash script program to perform matrix operations. Matrices are whitespace separated. 

Assignment Specs:

matrix dims [MATRIX]

	Prints error message to stderr, nothing to stdout and return value != 0 if:
	Argument count is greater than 1 (e.g. `matrix dims m1 m2`).
	Argument count is 1 but the file named by argument 1 is not readable (e.g. `matrix dims no_such_file`).
	Otherwise, prints "ROWS COLS" (Space separated!) to stdout, nothing to stderr, and returns 0.

matrix transpose [MATRIX]

	Prints error message to stderr, nothing to stdout and return value != 0 if:
	Argument count is greater than 1 (e.g. `matrix transpose m1 m2`).
	Argument count is 1 but the file named by argument 1 is not readable (e.g. `matrix transpose no_such_file`).
	Otherwise, prints the transpose of the input, in a valid matrix format to stdout, nothing to stderr, and returns 0.

matrix mean [MATRIX]

	Prints error message to stderr, nothing to stdout and return value != 0 if:
	Argument count is greater than 1 (e.g. `matrix mean m1 m2`).
	Argument count is 1 but the file named by argument 1 is not readable (e.g. `matrix mean no_such_file`).
	Otherwise, prints a row vector mean of the input matrix, in a valid matrix format to stdout, nothing to stderr, and returns 0. All values must round to the nearest integer, with ***.5 values rounded away from zero.

matrix add MATRIX_LEFT MATRIX_RIGHT

	Prints error message to stderr, nothing to stdout and return value != 0 if:
	Argument count does not equal 2 (e.g. `matrix add m1 m2 m3` or `matrix add m1`).
	Argument count is 2 but the file named by either argument is not readable (e.g. `matrix add m1 no_such_file`).
	The dimensions of the input matrices do not allow them to be added together following the rules of matrix addition.
	Otherwise, prints the sum of both matricies, in a valid matrix format to stdout, nothing to stderr, and returns 0.

matrix multiply MATRIX_LEFT MATRIX_RIGHT

	Prints error message to stderr, nothing to stdout and return value != 0 if:
	Argument count does not equal 2 (e.g. `matrix multiply m1 m2 m3` or `matrix multiply m1`).
	Argument count is 2 but the file named by either argument is not readable (e.g. `matrix multiply m1 no_such_file`).
	The dimensions of the input matrices do not allow them to be multiplied together following the rules of matrix multiplication.
	Otherwise, prints the product of both matricies, with the first argument as the left matrix and the second argumentas the right matrix, in a valid matrix format to stdout, nothing to stderr, and returns 0. (`matrix multiply A B` should return A*B, not B*A)
