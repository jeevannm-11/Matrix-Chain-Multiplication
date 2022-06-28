# Matrix-Chain-Multiplication
The code attached is used to find the most efficient way to multiply a sequence of matrices.
The problem here is not actually to perform the multiplications, but merely to decide in which order to perform the multiplications.

Illustration:
Input: p[] = {4, 2, 3, 1, 3}   
Output: 26
There are 4 matrices of dimensions 4x2, 2x3, 3x1 and 1x3.
Let the input 4 matrices be A, B, C and D.  The minimum number of 
multiplications are obtained by putting parenthesis in following way
(A(BC))D --> 2*3*1 + 4*2*1 + 4*1*3

Input: p[] = {1, 2, 3, 4, 3} 
Output: 30
There are 4 matrices of dimensions 1x2, 2x3, 3x4 and 4x3. 
Let the input 4 matrices be A, B, C and D.  The minimum number of 
multiplications are obtained by putting parenthesis in following way
((AB)C)D --> 1*2*3 + 1*3*4 + 1*4*3

Input: p[] = {1, 2, 3}  
Output: 6  
There are only two matrices of dimensions 10x20 and 20x30. So there 
is only one way to multiply the matrices, cost of which is 1*2*3
