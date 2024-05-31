SparseMatrix Class Documentation Overview The SparseMatrix class represents a sparse matrix, which is a matrix primarily composed of zero-valued elements. This class provides methods to initialize the matrix, load data from a file, set and get elements, and perform addition and subtraction with another sparse matrix.

Initialization init(self, numRows, numCols): Initializes the sparse matrix with the specified number of rows and columns. The matrix data is stored in a dictionary. Methods load_from_file(self, file_path): Loads matrix data from a file. The file should have the number of rows and columns on the first two lines, followed by the non-zero elements in (row, col, value) format.

set_element(self, row, col, value): Sets the element at the specified row and column to the given value.

get_element(self, row, col): Gets the element at the specified row and column. Returns 0 if the element is not set.

add(self, other): Adds the current matrix with another matrix and returns the result as a new SparseMatrix.

subtract(self, other): Subtracts another matrix from the current matrix and returns the result as a new SparseMatrix.

Example Usage Initialization: Create an instance of the SparseMatrix class by specifying the number of rows and columns.

Loading Data: Use the load_from_file method to load matrix data from a file.

Setting Elements: Use the set_element method to set specific elements in the matrix.

Getting Elements: Use the get_element method to retrieve specific elements from the matrix.

Matrix Addition: Use the add method to add two SparseMatrix instances and get the result.

Matrix Subtraction: Use the subtract method to subtract one SparseMatrix instance from another and get the result.

File Format for Loading Data The input file should contain:

The number of rows (rows=x) The number of columns (cols=y) The non-zero elements in the format (row, col, value)

Example Workflow Load Matrices: Load two sparse matrices from a file. Perform Operations: Add and subtract the matrices. Save Results: Save the results of the operations to output files.

Running the Script Save the script to a file. Run the script using a Python interpreter. The script will read the input file, perform the specified operations, and save the results to output files named output_add.txt and output_subtract.txt.
