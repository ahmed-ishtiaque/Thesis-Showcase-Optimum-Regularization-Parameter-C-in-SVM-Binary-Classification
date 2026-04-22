# SVM-OptiTune: Systematic Regularization via S&S Metric
> A high-efficiency alternative to k-fold Cross-Validation for Support Vector Machine (SVM) optimization.

## 📌 Project Overview
In SVM classification, the traditional default setting ($C=1$) or the fallback $k$-fold Cross-Validation (CV) creates a massive computational bottleneck. My research proposes a systematic approach that identifies the optimal $C$ in minutes rather than hours.

### Key Contributions:
* **S&S Metric:** Introduced a new "Separability & Scatteredness" metric to characterize dataset complexity.
<img width="651" height="538" alt="image" src="https://github.com/user-attachments/assets/6392c013-543f-4c7e-b6b6-d3b0fe4871d9" />
* **BVB C-Table:** Developed a lookup methodology based on the Bias-Variance trade-off.
 <img width="464" height="710" alt="Proposed Bias-Variance Based C Table" src="https://github.com/user-attachments/assets/61a6f8b6-40da-4f8c-905b-deac6e2a6a53" />

* **Performance:** Reduced optimization time significantly while maintaining accuracy.
  

## 📊 Results
Validated on synthetic and real-world datasets (Iris, Wine), the S&S method consistently identified the "Sweet Spot" of the Bias-Variance trade-off curve with zero manual iteration.
<img width="1287" height="994" alt="Comparing between Cross-validation result and Proposed Result" src="https://github.com/user-attachments/assets/411f128d-f795-497c-883f-3c365662f44b" />
Fig: Comparing between Cross-validation result and Proposed Result
<img width="1280" height="665" alt="Proposed Method on the Iris Flower Dataset" src="https://github.com/user-attachments/assets/3f84ebc3-68c4-40d7-b1ac-e07803dccc90" />
Fig: Applying Proposed Method on the Iris Flower Dataset
<img width="1272" height="712" alt="Comparing Proposed and CV result on Iris Flower Dataset" src="https://github.com/user-attachments/assets/18f5772a-5076-4019-93bf-a03f74cb848a" />
Fig: Comparing Proposed Method result and CV result on Iris Flower Dataset

## 🎓 Academic Record
* **Thesis:** [Optimum Regularization Parameter C in SVM Binary Classification](https://doi.org/10.32920/24050733.v1)
* **University:** Ryerson University, Toronto, ON.
* **Researcher:** Ishtiaque Ahmed
