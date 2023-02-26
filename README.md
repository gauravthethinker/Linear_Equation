# Solving linear equation using SVD decomposition  

Procedure to find solution:
1. take svd of matrix A  u,sigma,vt  =svd(A)
2. find inverse of sigma using r. that inv_sigma
3. make diagonal matrix with inv_sigma ie. diag(inv_sigma)
4.multiply vt.T, diag(inv_sigma), u.T and b
5. Take norm of |A*x-b||**2
