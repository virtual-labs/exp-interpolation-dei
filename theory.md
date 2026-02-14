## Theory  

Interpolation is a fundamental numerical technique used to construct an approximate function 
𝑃𝑛(𝑥)that passes exactly through a given set of data points:

<img width="248" height="37" alt="image" src="https://github.com/user-attachments/assets/ad1ea27c-1da2-4e1a-8c13-399c8b7fcbe5" />

where yi​=f(xi​), The objective is to estimate unknown values of the function within the range of the known data. Unlike regression, interpolation assumes that the approximating curve passes exactly through all provided points.

In general, for n+1 distinct data points, there exists a unique polynomial of degree at most 𝑛 that interpolates the data.
Interpolation is a numerical technique used to estimate unknown values of a function based on a finite set of known data points. It is especially useful when the functional relationship between variables is unknown and experimental or sampled data is available.

In this experiment, three interpolation methods are used, each differing in complexity and accuracy.


### General Form of Interpolation Polynomial

The interpolating polynomial of degree 𝑛 can be expressed as:

<img width="359" height="36" alt="image" src="https://github.com/user-attachments/assets/298e4ce7-de3b-4d08-8080-f25a22ae991c" />

The interpolation error at any point 𝑥 is given by:

<img width="479" height="73" alt="image" src="https://github.com/user-attachments/assets/eb5abda5-dfdd-4290-ab2f-e89643f94fc4" />

where 𝜉 lies in the interval containing the data points.

This expression shows that:

- Error increases with higher derivatives.

- Error depends strongly on spacing of data points.

- Degree of polynomial affects numerical stability.


### 1. Linear Interpolation  
<img width="988" height="204" alt="image" src="https://github.com/user-attachments/assets/4472aedf-06d1-498f-b255-b030e1159c5e" />

Key characteristics:

- Uses only two nearest data points

- Easy to implement

- Less accurate for nonlinear data

This method is suitable when data points are closely spaced and the function varies smoothly.

### 2. Lagrange Interpolation
<img width="976" height="245" alt="image" src="https://github.com/user-attachments/assets/7f68a8d4-9971-4fb1-8ba7-5a0e1ba9a377" />

Key characteristics:

- Works for unevenly spaced data

- Produces exact fit for given points

- Polynomial degree increases with number of points

This method is widely used when a global interpolation across all data points is required.

### 3. Newton’s Divided Difference Method
<img width="961" height="334" alt="image" src="https://github.com/user-attachments/assets/b3103f2b-d3d4-42fa-901a-b276b47472d3" />

Key characteristics:

- Efficient for adding new data points

- Numerically stable compared to Lagrange for large datasets

- Suitable for computational implementation


### Evenly vs. Unevenly Spaced Data  
- For **evenly spaced points**, Newton’s Forward and Backward methods are efficient and computationally straightforward.  
- For **unevenly spaced points**, generalized approaches such as Lagrange and Newton’s Divided Difference methods are more appropriate.  

---

### Learning Outcomes from This Experiment  
By performing this experiment, learners will be able to:  
- Analyze the **accuracy** of different interpolation methods.  
- Compare their **computational efficiency**.  
- Select the most **suitable method** depending on the dataset type.  
- Understand real-world applications in **signal processing, image scaling, weather forecasting, biomedical data, and machine learning preprocessing**.  

Interpolation is not just a mathematical tool but a **bridge between discrete data and continuous analysis**, making it a cornerstone in modern computational sciences.  
