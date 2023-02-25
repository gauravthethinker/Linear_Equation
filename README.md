# Linear_Equation
The LinearSystem class takes an input matrix A in its constructor, which is stored as an instance variable. 
The solve method takes a right-hand side vector b and computes the least-squares optimal solution a using the QR factorization of A. 
The QR factorization is computed only once and then reused for subsequent solves.

The save and load methods use the pickle module to serialize and deserialize the instance of the LinearSystem class to a file. 
This allows the state of the linear system to be saved and loaded later, for example, when training a machine learning model that requires 
solving the same linear system multiple times.

Finally, the residual_norm method computes the norm of the residual |Aa - b| for a given solution a and right-hand side b.
