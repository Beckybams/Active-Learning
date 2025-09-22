** Active Learning with Synthetic Data

This project demonstrates **Active Learning** using a synthetic 2D dataset for binary classification.  
Active Learning allows a model to learn efficiently by selecting the most *informative* samples to label instead of labeling everything at once.

---

## 📂 Files

- **`synthetic_active_learning_data.xlsx`**  
  Synthetic dataset with two features and a binary label.

- **`active_learning_synthetic.py`**  
  Python script that:
  - Generates synthetic data  
  - Initializes with a small labeled set  
  - Iteratively queries the most uncertain unlabeled points  
  - Retrains the model with the newly labeled data  
  - Visualizes the decision boundary  
  - Plots accuracy vs. number of labeled samples  

---

## ⚙️ Requirements

Install dependencies with:

```bash
pip install numpy pandas scikit-learn matplotlib
▶️ How to Run
bash
Copy code
python active_learning_synthetic.py
The script will:

Print accuracy at each iteration

Show evolving decision boundaries

Save the dataset to Excel

📊 Results
The model starts with only a few labeled points → low accuracy

As it queries uncertain samples → accuracy improves

Final output includes:

Visualization of decision boundary at each step

A learning curve of accuracy vs labeled set size

🔧 Customization
You can change:

Dataset parameters (n_samples, class_sep)

Active learning settings (initial_samples, batch_size, n_queries)

Query strategies (uncertainty, margin, entropy)

📖 Reference
Becky bbpere07@gmail.com
Scikit-learn Documentation

