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

### Summary Plot - Bar 
![Screenshot 2023-05-25 at 8 48 45 PM](https://github.com/sharclark/Project-1-Revisited.ipynb/assets/123594410/2ff83365-b386-486a-b82e-368a2c61517d)

- The top 5 features for the Shap Summary are as follows:
    1. Item_MRP
    2. Outlet_Type_Grocery Store
    3. Outlet_Type_SuperMarket Type 3
    4. Outlet_Establishment_Year
    5. Item_Visibility
    
- The top 5 Features for the Feature Importance are as follows:
    1. Item_MRP
    2. Outlet_Type Grocery Store
    3. Item Visibility
    4. Outlet_Type_SuperMarket Type 3
    5. Item_Weight

Item Visiblity is higher on the feature importances and Item weight has been included. Establishment Year is included in the Shap summary, but not the Feature Importance.

### Summary Plot - Dot
![Screenshot 2023-05-25 at 8 50 10 PM](https://github.com/sharclark/Project-1-Revisited.ipynb/assets/123594410/47c30eeb-3ff8-4db8-9f52-ff98cd7ec66e)
- Item MRP - The more Item_MRP the higher predicted sales.
-  Outlet_Type_Grocery Store - The lower the values in Grocery Store, the higher the predicted price.
-  Outlet_Type_SuperMarket Type 3 - The higher the values in Outlet_Type_SuperMarket Type 3 the higer the sales.

### Shap Force Plot - Max Year
![Screenshot 2023-05-25 at 9 35 15 PM](https://github.com/sharclark/Project-1-Revisited.ipynb/assets/123594410/4d83b5b6-174e-48d1-84c5-b59e1d5501c6)
 - The Item weight, outlet type, and item MRP is pushing the sale value higher, and the outlet type 3, Establishment year, and item visibility are pushing the value down. 
 
### Shap Force Plot - Min Year
![Screenshot 2023-05-25 at 9 39 21 PM](https://github.com/sharclark/Project-1-Revisited.ipynb/assets/123594410/f8095eee-73d9-449c-953c-c0fb3c1311b6)
- - The year and outlet type_3 are pushing the sales higher, and the item_MRP are pushing the sales lower.

### Lime Explanation - Max Year
![Screenshot 2023-05-25 at 9 45 59 PM](https://github.com/sharclark/Project-1-Revisited.ipynb/assets/123594410/a92a803f-66a7-42bb-857f-b444fe0a7746)
- This lime explainer is showing that Outlet_type_Grocery store had the highest positive impact on predicting the sales for this model. However, the fact that Outlet_type_supermarket was lower than 1107 impacted the sales negatively. 

### Lime Explanation - Min Year
![Screenshot 2023-05-25 at 9 51 27 PM](https://github.com/sharclark/Project-1-Revisited.ipynb/assets/123594410/676056f8-88fd-4558-b4c0-5493a205fb8b)

- This lime explainer shows that Outlet_Type_Grocery Store had the highest positive impact on sales. But because the MRP was lower than 98.82 it decreased the sales. 
