### Procedure

1. Open the simulation interface for the interpolation experiment.

2. From the **Interpolation Method** dropdown menu, select one of the following options:
   - Linear Interpolation  
   - Lagrange Interpolation  
   - Newton’s Divided Differences  

3. Enter the known data points in the input field using the prescribed format:  
   **Format:** `x1,y1; x2,y2; x3,y3; ...`  
   *(Example: `1,2; 2,4; 3,6`)*  

   Ensure that:
   - Each data pair is separated by a semicolon (`;`)
   - The x and y values within a pair are separated by a comma (`,`)

4. Enter the value of the independent variable at which interpolation is required.

5. Click the **Submit** button to perform the interpolation.

6. **Observation:**
   - Observe the interpolated value displayed as output.
   - For **Linear Interpolation**, note that the result is computed using only the two nearest data points.
   - For **Lagrange Interpolation** and **Newton’s Divided Difference** methods, note that all provided data points are used to construct the interpolating polynomial.
   - Compare the interpolated values obtained using different methods for the same dataset.

7. Repeat the experiment by changing:
   - The interpolation method
   - The number of data points
   - The interpolation value  

   to analyze the effect on the interpolated result.
