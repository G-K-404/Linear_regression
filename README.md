<h1>📈 Linear Regression from Scratch in Python</h1>
This project demonstrates a complete implementation of univariate linear regression using both Gradient Descent and Stochastic Gradient Descent (SGD). It includes data normalization, model training, evaluation using accuracy metrics like R² and MSE, and visualization of predicted vs actual outputs.

<h2>🔧 Features</h2>
<h3>Linear regression using:</h3>

Batch Gradient Descent

Stochastic Gradient Descent (SGD)

<h3>Works on both:</h3>

Custom dummy data(with significant R^2 value)

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
```plaintext
Path: ./archive2/Salary_dataset.csv
Format: CSV with two columns:

YearsExperience (independent variable x)

Salary (dependent variable y)
```
<a href="https://www.kaggle.com/datasets/abhishek14398/salary-dataset-simple-linear-regression/data">Dataset</a>
<h3>🚀 How It Works</h3>
<h4>🔁 Model Equation</h4>
The prediction function is:
```equation
ŷ = w1 + w2 * x
Where:

w1 is the bias

w2 is the weight

x is the input feature
```
<h4>🔍 Cost Function</h4>
The loss is measured using the Mean Squared Error (MSE):
```
MSE = (1/N) * Σ(ŷ - y)²
```
<h3>🧠 Optimization Methods</h3>
<h4>✅ Batch Gradient Descent</h4>
Updates parameters using the average gradient over the full dataset.

<h4>🔄 Stochastic Gradient Descent (SGD)</h4>
Updates weights for each data point one at a time — faster, more volatile convergence.

<h3>📈 Visualization</h3>
Plots are created using Matplotlib to show:

Original data (scatter plot)

Predicted line (regression line)

📊 Accuracy Metrics
R² Score: Measures how well predictions match actual values.

R² = 1 - (SSR/SST)

Mean Squared Error (MSE): Measures average squared difference between predicted and actual values.

<h2>⚙️ Usage</h2>
<h3>1. Clone the Repository</h3>
```bash
git clone https://github.com/yourusername/linear-regression-scratch.git
cd linear-regression-scratch
```
<h3>2. Run the Notebook or Script</h3>
Ensure matplotlib and numpy are installed:
```bash
pip install matplotlib numpy
```
Then run using Jupyter Notebook or directly execute the Python script.

<h2>🧪 Example Results</h2>
<h3>Using dummy data:</h3>

```yaml
Input: x = [1,2,3,...,10]
Output: y = [5,7,9,...,23]

Gradient Descent:
R² ≈ 1.0
MSE ≈ very low

SGD:
R² ≈ 0.999
MSE ≈ slightly higher
Using real dataset (Salary_dataset.csv):
```
Scaled data (mean-std normalization)

R² ≈ high (close to 0.9+ depending on data quality)

<h2>📌 Notes</h2>
Normalize inputs for better convergence.

Learning rate and epoch count highly affect convergence.

SGD gives quicker but noisier convergence compared to batch gradient descent.

