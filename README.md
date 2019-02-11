# Assignment-5
A <- matrix(1:100, nrow = 10)
B <- matrix(1:10000, nrow=100)
det (A) # determinant is equal to zero 
det (B) # determinant is equal to zero 
solve (A) # this is a singular (non invertable) matrix
solve (B) # this is a rectangular and non invertable matrix

# The generalized inverse (or pseudoinverse) package may help us to solve the problem.
# However, in this assignment we multiply the matrices by vectors with respective number of columns to generate invertible matrices.

# I tried all the possible but still the determinant remains zero!
A <- matrix(1:100, nrow = 10)
B<- matrix(1:1000, nrow=10)
AB= A %*% B
TB= t(B)
TBAB= TB%*%AB
det(TBAB)
solve(TBAB)