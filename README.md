# SVM-OptiTune: Systematic Regularization via S&S Metric
> A high-efficiency alternative to k-fold Cross-Validation for Support Vector Machine (SVM) optimization.

## 📌 Project Overview
In SVM classification, the traditional default setting ($C=1$) or the fallback $k$-fold Cross-Validation (CV) creates a massive computational bottleneck. My research proposes a systematic approach that identifies the optimal $C$ in minutes rather than hours.

### Key Contributions:
* **S&S Metric:** Introduced a new "Separability & Scatteredness" metric to characterize dataset complexity.
* **BVB C-Table:** Developed a lookup methodology based on the Bias-Variance trade-off.
* **Performance:** Reduced optimization time from ~2 hours to <2 minutes while maintaining accuracy.

## 📊 Results
Validated on synthetic and real-world datasets (Iris, Wine), the S&S method consistently identified the "Sweet Spot" of the Bias-Variance trade-off curve with zero manual iteration.
<img width="1287" height="994" alt="Comparing between Cross-validation result and Proposed Result" src="https://github.com/user-attachments/assets/411f128d-f795-497c-883f-3c365662f44b" />
<img width="1287" height="994" alt="Proposed Bias-Variance Based C Table" src="https://github.com/user-attachments/assets/f0a7f65d-0457-4df0-b70f-135474e75614" />
<img width="1287" height="994" alt="Proposed Method on the Iris Flower Dataset" src="https://github.com/user-attachments/assets/ab03b1be-2120-4f08-a54e-72e5e58f308a" />
<img width="1287" height="994" alt="Comparing Proposed and CV result on Iris Flower Dataset" src="https://github.com/user-attachments/assets/4e7fd869-d590-492c-9784-1bd86d2b744f" />

## 🎓 Academic Record
* **Thesis:** [Optimum Regularization Parameter C in SVM Binary Classification](https://doi.org/10.32920/24050733.v1)
* **University:** Ryerson University, Toronto, ON.
* **Researcher:** Ishtiaque Ahmed
