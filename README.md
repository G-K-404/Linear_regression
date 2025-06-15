<h1>📈 Linear Regression from Scratch in Python</h1>
This project demonstrates a complete implementation of univariate linear regression using both Gradient Descent and Stochastic Gradient Descent (SGD). It includes data normalization, model training, evaluation using accuracy metrics like R² and MSE, and visualization of predicted vs actual outputs.

<h2>🔧 Features</h2>
Linear regression using:

Batch Gradient Descent

Stochastic Gradient Descent (SGD)

Works on both:

Custom dummy data

Real dataset (Salary_dataset.csv)

Data normalization (mean-standard deviation scaling)

Visualization using Matplotlib

Performance evaluation via:

R² Score (Coefficient of Determination)

Mean Squared Error (MSE)

<h2>📂 File Structure</h2>
```plaintext
project/
│
├── archive2/
│   └── Salary_dataset.csv   
│
├── linear_regression.py    
├── README.md                

```
<h2>📊 Dataset</h2>
Path: ./archive2/Salary_dataset.csv
Format: CSV with two columns:

YearsExperience (independent variable x)

Salary (dependent variable y)

🚀 How It Works
🔁 Model Equation
The prediction function is:

Copy
Edit
ŷ = w1 + w2 * x
Where:

w1 is the bias

w2 is the weight

x is the input feature

🔍 Cost Function
The loss is measured using the Mean Squared Error (MSE):

ini
Copy
Edit
MSE = (1/N) * Σ(ŷ - y)²
🧠 Optimization Methods
✅ Batch Gradient Descent
Updates parameters using the average gradient over the full dataset.

🔄 Stochastic Gradient Descent (SGD)
Updates weights for each data point one at a time — faster, more volatile convergence.

📈 Visualization
Plots are created using Matplotlib to show:

Original data (scatter plot)

Predicted line (regression line)

📊 Accuracy Metrics
R² Score: Measures how well predictions match actual values.

R² = 1 - (SSR/SST)

Mean Squared Error (MSE): Measures average squared difference between predicted and actual values.

⚙️ Usage
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/yourusername/linear-regression-scratch.git
cd linear-regression-scratch
2. Run the Notebook or Script
Ensure matplotlib and numpy are installed:

bash
Copy
Edit
pip install matplotlib numpy
Then run using Jupyter Notebook or directly execute the Python script.

🧪 Example Results
Using dummy data:

yaml
Copy
Edit
Input: x = [1,2,3,...,10]
Output: y = [5,7,9,...,23]

Gradient Descent:
R² ≈ 1.0
MSE ≈ very low

SGD:
R² ≈ 0.999
MSE ≈ slightly higher
Using real dataset (Salary_dataset.csv):

Scaled data (mean-std normalization)

R² ≈ high (close to 0.9+ depending on data quality)

📌 Notes
Normalize inputs for better convergence.

Learning rate and epoch count highly affect convergence.

SGD gives quicker but noisier convergence compared to batch gradient descent.

