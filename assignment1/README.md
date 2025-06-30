# Assignment 1 — Linear Algebra Foundations

**Student:** `<Your Name>`  
**Dartmouth ID:** `<Your ID>`

---

## Objective

In this assignment, we will review and implement key linear algebra operations from scratch using Python — including:

- Matrix multiplication
- Matrix inverse
- Singular Value Decomposition (SVD)
- Pseudo-inverse

These exercises reinforce theoretical concepts and introduce key NumPy/SciPy functions used throughout applied machine learning.

---

## Section 1: Matrix Multiplication

To multiply a matrix by another, we take the **dot product** of the rows of the first matrix with the columns of the second. For this to be valid:

> The **number of columns in the first matrix** must equal the **number of rows in the second**.

This produces a new matrix with:
- Rows = number of rows in the first matrix
- Columns = number of columns in the second matrix

**Instructions:**
- Implement the function `matrix_multiplication(matrix1, matrix2)`
- Do not use built-in matrix multiplication for your core function
- Test your implementation using built-in alternatives like:
  - `np.dot(matrix1, matrix2)`
  - `np.matmul(matrix1, matrix2)`
  - `matrix1 @ matrix2`

---

## Section 2: Matrix Inverse

The inverse of a matrix `A` is denoted as `A⁻¹` and is defined such that:

> `A @ A⁻¹ = I` (where `I` is the identity matrix)

Note that not all matrices have an inverse (non-invertible or singular matrices).

**Instructions:**
- Implement the function `matrix_inverse(matrix)`
- Build this from first principles if possible (row reduction, etc.)
- Test your result using:
  - `np.linalg.inv(matrix)`
  - `scipy.linalg.inv(matrix)`

---

## Section 3: Singular Value Decomposition (SVD)

SVD decomposes a matrix `A` as:

> `A = U Σ Vᵀ`

Where:
- `U` and `Vᵀ` are orthogonal
- `Σ` is a diagonal matrix of singular values

SVD is widely used in data compression, dimensionality reduction, and signal processing.

**Instructions:**
- Implement `matrix_svd(matrix)`
- Output should be: `U, sigma, V.T`
- Check results with:
  - `np.linalg.svd(matrix)`
  - `scipy.linalg.svd(matrix)`

---

## Section 4: Matrix Pseudo-Inverse

The pseudo-inverse is used to solve linear systems when the inverse doesn’t exist or the matrix is not square.

**Instructions:**
- Implement `matrix_pseudo_inverse(matrix)`
- Assume the matrix is square and invertible
- For validation, try:
  - `np.linalg.pinv(matrix)`
  - `scipy.linalg.pinv(matrix)`

---

## Notes

- You may import other standard libraries if needed
- Use assertions or visual checks to confirm that your results match built-in function outputs
- Submit this file as a completed Jupyter Notebook through GitHub Classroom
- You are encouraged to explore beyond what's provided!

---

**Happy coding!**  
`<Your Name>`  
`<Your ID>`

