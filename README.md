
# Monte Carlo Estimation of π  

## Overview  
This project demonstrates how the **Monte Carlo simulation method** can be used to approximate the value of π using MATLAB. The method works by randomly generating points inside a square and checking how many of them fall within a quarter circle drawn inside that square. By comparing the ratio of inside points to the total points, we can estimate π.  

The project is divided into three tasks that gradually build on one another:  

- **Task 1 – For Loop with Fixed Points:** Estimate π using different fixed sample sizes and show how accuracy improves with more points.  
- **Task 2 – While Loop with Precision Target:** Keep generating points until the estimate stabilizes at the required precision.  
- **Task 3 – Function with Visualization:** Wrap the logic into a reusable function with interactive scatter plots to show points as they are generated.  

This step-by-step approach illustrates not only the idea of Monte Carlo simulation but also how programming structures (loops, functions, plotting) can be applied to solve numerical problems.  

---

## Task Explanations  

### 🔹 Task 1: For Loop with Fixed Number of Points  
- A list of sample sizes (e.g., 10, 100, 1000, 10000) is used.  
- For each size, random points are generated inside the square.  
- The program counts how many points fall inside the quarter circle.  
- The estimate of π is calculated and compared to the true value.  
- Three plots are created:  
  1. Estimated π vs. number of points  
  2. Error vs. number of points  
  3. Runtime vs. number of points  

This task shows the trade-off: more points improve accuracy but take longer to compute.  

---

### 🔹 Task 2: While Loop with Precision Target  
- Instead of fixing the number of points, the program continues until the π estimate stabilizes.  
- The user sets a precision (e.g., 3 significant figures).  
- Points are generated in batches, and after each batch the π estimate is updated.  
- If the rounded value matches the previous result for several consecutive rounds, the simulation stops.  
- The program then prints the final estimate, the rounded value, and how many total points were required.  

This task is more practical, because it stops automatically once the result is “good enough.”  

---

### Task 3: Function with Visualization  
- The logic from Task 2 is wrapped into a function: `piii_value_func(k)` where `k` is the desired precision.  
- Random points are shown on a live scatter plot:  
  - Blue = inside the quarter circle  
  - Red = outside the circle  
- The plot is updated as more points are generated.  
- When stable, the program prints the final π estimate in the Command Window and shows the rounded result on the plot.  

This task makes the program user-friendly and visually interactive.  

---

##  Requirements  
- **MATLAB R2020a or newer**  
- Project scripts:  
  - `sachdeva_prerna_project1.m` — runs **Task 1**
