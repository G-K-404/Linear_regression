<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
</head>
<body>

<h1>Linear Regression from Scratch in Python 📈</h1>

<p>This project demonstrates a complete implementation of univariate linear regression using both Gradient Descent and Stochastic Gradient Descent (SGD). It includes data normalization, model training, evaluation using accuracy metrics like R² and MSE, and visualization of predicted vs actual outputs.</p>

<h2>🔧 Features</h2>

<h3>Linear regression using:</h3>
<ul>
  <li>Batch Gradient Descent</li>
  <li>Stochastic Gradient Descent (SGD)</li>
</ul>

<h3>Works on both:</h3>
<ul>
  <li>Custom dummy data (with significant R² value)</li>
  <li>Real dataset (<code>Salary_dataset.csv</code>)</li>
</ul>

<ul>
  <li>Data normalization (mean-standard deviation scaling)</li>
  <li>Visualization using Matplotlib</li>
</ul>

<h4>Performance evaluation via:</h4>
<ul>
  <li>R² Score (Coefficient of Determination)</li>
  <li>Mean Squared Error (MSE)</li>
</ul>

<h2>📂 File Structure</h2>

<pre><code>project/
│
├── archive2/
│   └── Salary_dataset.csv   
│
├── linear_regression.py    
├── README.md
</code></pre>

<h2>📊 Dataset</h2>

<pre><code>Path: ./archive2/Salary_dataset.csv
Format: CSV with two columns:

- YearsExperience (independent variable x)
- Salary (dependent variable y)
</code></pre>

<p><a href="https://www.kaggle.com/datasets/abhishek14398/salary-dataset-simple-linear-regression/data" target="_blank">🔗 Dataset Source (Kaggle)</a></p>

<h2>🚀 How It Works</h2>

<h3>🔁 Model Equation</h3>
<pre><code>ŷ = w1 + w2 * x

Where:
w1 is the bias
w2 is the weight
x is the input feature
</code></pre>

<h3>🔍 Cost Function</h3>
<pre><code>MSE = (1/N) * Σ(ŷ - y)²
</code></pre>

<h2>🧠 Optimization Methods</h2>

<h4>✅ Batch Gradient Descent</h4>
<p>Updates parameters using the average gradient over the full dataset.</p>

<h4>🔄 Stochastic Gradient Descent (SGD)</h4>
<p>Updates weights for each data point one at a time — faster, more volatile convergence.</p>

<h2>📈 Visualization</h2>

<p>Plots are created using Matplotlib to show:</p>
<ul>
  <li>Original data (scatter plot)</li>
  <li>Predicted line (regression line)</li>
</ul>

<h3>📊 Accuracy Metrics</h3>
<ul>
  <li><strong>R² Score:</strong> Measures how well predictions match actual values.<br>
  R² = 1 - (SSR/SST)</li>
  <li><strong>Mean Squared Error (MSE):</strong> Measures average squared difference between predicted and actual values.</li>
</ul>

<h2>⚙️ Usage</h2>

<h3>1. Clone the Repository</h3>
<pre><code>git clone https://github.com/yourusername/linear-regression-scratch.git
cd linear-regression-scratch
</code></pre>

<h3>2. Run the Notebook or Script</h3>
<p>Ensure matplotlib and numpy are installed:</p>

<pre><code>pip install matplotlib numpy
</code></pre>

<p>Then run using Jupyter Notebook or directly execute the Python script.</p>

<h2>🧪 Example Results</h2>

<h3>Using dummy data:</h3>
<pre><code>Input: x = [1,2,3,...,10]
Output: y = [5,7,9,...,23]

Gradient Descent:
R² ≈ 1.0
MSE ≈ very low

SGD:
R² ≈ 0.999
MSE ≈ slightly higher
</code></pre>

<h3>Using real dataset (Salary_dataset.csv):</h3>
<ul>
  <li>Scaled data (mean-std normalization)</li>
  <li>R² ≈ high (close to 0.9+ depending on data quality)</li>
</ul>

<h2>📌 Notes</h2>
<ul>
  <li>Normalize inputs for better convergence.</li>
  <li>Learning rate and epoch count highly affect convergence.</li>
  <li>SGD gives quicker but noisier convergence compared to batch gradient descent.</li>
</ul>

</body>
</html>
