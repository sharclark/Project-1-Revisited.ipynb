# Outlet Sales - Revisited.ipynb

Shar Clark

## Machine Learning using the following models:
   - Linear Regression Model
   - Decision Tree Model

### Linear Regression Coefficients Plot

![Screenshot 2023-05-25 at 8 36 46 PM](https://github.com/sharclark/Project-1-Revisited.ipynb/assets/123594410/155911f9-7a13-4e33-8f30-b6ea042e5b45)

- The highest coefficient is Outlet_Type_SuperMarket Type 3. Our data was not scaled, so this shows that if the outlet type matches this, it increases sales by an average of $1984.76. 
- The second highest coefficient is Outlet_Size_High. This shows that if that is the outlet size, sales were increased by an average of $495.82
- The third highest coefficient is Outlet_Type_SuperMarket Type 2. This had a negative correlation. If this is the outlet type the sales were decreased by an average of $402.58. 

### Random Forest Feature Importances
<img width="899" alt="Screenshot 2023-05-25 at 8 43 54 PM" src="https://github.com/sharclark/Project-1-Revisited.ipynb/assets/123594410/a7409605-dfc6-490e-b3b1-fa06c4ce26b7">

- The most important feature according to the Random Forest model was Item_MRP. This was not in the Linear Regression Coefficients. 
- Item Weight is the 5th most important feature according to our Random Forest Model. This was also nt in the Linear Regression Coefficients. 
- The other 3 features are in the top 5 of both models. 
