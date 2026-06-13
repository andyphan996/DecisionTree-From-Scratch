# Decision Tree from Scratch vs. Scikit-Learn

A Python implementation of a **Decision Tree Classifier built from scratch** using only `NumPy`, evaluated and benchmarked against `scikit-learn`'s standard implementation on the continuous **Iris Dataset**.

---

## 📌 Project Overview
The goal of this project is to demystify how Decision Trees operate under the hood. Instead of relying purely on high-level libraries, this project implements the mathematical foundation of the algorithm—including Gini impurity, continuous feature splitting, and recursive tree construction—and measures its correctness against an industry-standard library.

## 🚀 Features
* **Built from Scratch:** Pure `NumPy` implementation without high-level ML framework dependencies.
* **Continuous Feature Handling:** Dynamically calculates binary thresholds for continuous variables (e.g., Iris petal/sepal measurements).
* **Evaluation & Benchmark:** Side-by-side accuracy and structure comparison with `scikit-learn`.
* **Tree Visualization:** Includes a custom text-based tree printing method (`print_tree`) alongside `scikit-learn`'s `plot_tree`.

## 📊 Results & Evaluation
After splitting the Iris dataset into training (80%) and testing (20%) sets, both models were restricted to a `max_depth=3` to ensure a fair evaluation. 

### Model Performance
| Model Implementation | Test Accuracy |
| :--- | :--- |
| **My Decision Tree (From Scratch)** | **80.0%** |
| **Scikit-Learn (`DecisionTreeClassifier`)** | **80.0%** |

### Key Takeaways
1. **Algorithmic Correctness:** The identical **80.0% accuracy score** validates that our custom implementation's core logic—Gini index calculation, recursive tree building, and continuous feature splitting—functions flawlessly and aligns with production-grade frameworks.
2. **Efficiency vs. Transparency:** While `scikit-learn` offers faster execution and advanced hyperparameter tuning, building the model from scratch provides unparalleled transparency into how decision boundaries are mathematically established.

## 🛠️ Installation & Usage
To run the notebook locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone [https://github.com/andyphan996/DecisionTree-From-Scratch.git](https://github.com/andyphan996/DecisionTree-From-Scratch.git)
Install the required libraries:

Bash
pip install numpy scikit-learn matplotlib jupyter
Open and run the Jupyter Notebook:

Bash
jupyter notebook
