# SVM-OptiTune: Systematic Regularization via S&S Metric
> A high-efficiency alternative to k-fold Cross-Validation for Support Vector Machine (SVM) optimization.
## 📌 Project Overview
In SVM classification, the traditional default setting ($C=1$) or the fallback $k$-fold Cross-Validation (CV) creates a massive computational bottleneck. My research proposes a systematic approach that identifies the optimal $C$ in minutes rather than hours.

### Key Contributions:
* **S&S Metric:** Introduced a new "Separability & Scatteredness" metric to characterize dataset complexity.
* **BVB C-Table:** Developed a lookup methodology based on the Bias-Variance trade-off.
* **Performance:** Reduced optimization time from ~2 hours to <2 minutes while maintaining or improving accuracy.
## ⚙️ How It Works
The workflow follows a 3-step systematic rule to bypass iterative testing:

```mermaid
graph TD
    A[Dataset Input] --> B[Step 1: Calculate S&S Metric]
    B --> C{Is S&S >= 5.68?}
    C -->|Yes: Separable| D[Use Generalized MAV Equation]
    C -->|No: Overlapping| E[Lookup BVB C-Table]
    D --> F[Output Optimal C]
    E --> F
    F --> G[Train SVM Model]

## 🚀 Getting Started

### Prerequisites
* Python 3.8+
* Scikit-learn, Pandas, NumPy

### Usage
```python
from svm_optimizer import calculate_ss, get_optimum_c

# 1. Calculate the S&S factor for your training data
ss_factor = calculate_ss(X_train, y_train)

# 2. Retrieve the optimal C based on the BVB logic
optimal_c = get_optimum_c(ss_factor)

## 📊 Results
Validated on synthetic and real-world datasets (Iris, Wine), the S&S method consistently identified the "Sweet Spot" of the Bias-Variance trade-off curve with zero manual iteration.

## 🎓 Academic Record
* **Thesis:** [Optimum Regularization Parameter C in SVM Binary Classification](https://doi.org/10.32920/24050733.v1)
* **University:** Ryerson University, Toronto, ON.
* **Researcher:** Ishtiaque Ahmed, P.Eng.
