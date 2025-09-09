Project Report: Linear Regression from Scratch — Closed-form vs Gradient Descent
## Student Info :  
Name: Rohith Varma Suraparaju  
Student ID: 700771851  
Assignment: # Gradient-Descent-for-Linear-Regression
Implementation of Linear Regression from scratch using Closed-form solution and Gradient Descent, with dataset generation, plots, and comparison of results. 

---

## 📖 Problem Statement  
To implement Linear Regression using Gradient Descent from scratch (without using scikit-learn’s `LinearRegression`).  
Task is to compare the Closed-form solution (Normal Equation) with Gradient Descent on the same dataset.  
compare both methods on the same synthetic dataset and analyze if Gradient Descent converges to the same solution as the Normal Equation.

---

## 📊 Dataset  
We generate a synthetic dataset of 200 samples:  
y = 3 + 4x + epsilon}

- (x in [0, 5]) uniformly sampled  
- (epsilon) is Gaussian noise  

---

##  Implementation Steps  

### 1. Dataset Generation
- Created 200 samples.  
- Added Gaussian noise.  
- Plotted raw data.  

### 2. Closed-form Solution (Normal Equation)
- Added bias column of 1’s to \(X\).  
- Computed parameters using:  
  \theta = (X^TX)^{-1}X^Ty
- Printed intercept & slope.  
- Plotted fitted line with raw data.  

### 3. Gradient Descent
- Initialized \(\theta = [0, 0]\).  
- Learning rate: \(\eta = 0.05\).  
- Iterations: 1000.  
- Plotted loss curve (MSE vs iterations).  
- Printed final intercept & slope.  

### 4. Comparison
- Reported parameters from both methods.  
- Checked convergence.  

---

## 📈 Results  

**Closed-form Solution:**  
- Intercept = 2.6908  
- Slope = 4.1318 

**Gradient Descent Solution:**  
- Intercept = 2.6908
- Slope = 4.1318

✅ Both methods converged to nearly the same solution.  

---

## 📝 Short Explanation  
Both the closed-form solution and Gradient Descent produced nearly identical parameters (intercept ≈ 2.69, slope ≈ 4.13). This confirms that Gradient Descent successfully converged to the same optimal solution as the Normal Equation, since both minimize the same convex MSE cost function.  

