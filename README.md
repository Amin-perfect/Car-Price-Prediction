# Used Car Price Prediction
 
A regression model that predicts a used car's resale price based on its age, mileage, fuel type, transmission, and ownership history built during the CodeAlpha Data Science Internship.
 
## Why this problem matters
Used car pricing depends on multiple interacting factors that aren't obvious at a glance a car's age matters differently depending on its mileage and fuel type. This project models those interactions to produce a data-driven price estimate instead of a rough guess.
 
## Approach
- Cleaned the dataset and handled categorical features (fuel type, seller type, transmission, owner) using feature encoding
- Performed correlation analysis to identify which features most influenced selling price
- Split data into training and test sets
- Trained a **Linear Regression** model on the encoded features
- Evaluated performance using R² score
## Result
The model achieved an **R² score of 0.78** on the test set, meaning it explains 78% of the variance in selling price based on the car's features alone.
 
## Tech Stack
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Jupyter Notebook
 
## Project Structure
```
CodeAlpha_CarPricePrediction/
├── dataset/
├── notebook/
├── images/
├── README.md
└── requirements.txt
```
 
## Author
Amin (Mr. PerfecT)  BSCS Student | Aspiring Data Scientist & AI Developer
 
