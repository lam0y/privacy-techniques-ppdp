# Privacy-Preserving Data Publishing Techniques

This repository contains the code and experiments for a project evaluating three Privacy-Enhancing Techniques (PETs) for Privacy-Preserving Data Publishing (PPDP): **Anonymization**, **Synthetic Data Generation**, and **Differential Privacy**.

The project was conducted as part of an internship at **Université de Sherbrooke**, under the supervision of **Professor Pierre-Martin Tardif**.

---

## 📌 Project Objectives

- To explore and implement various Privacy Enhancing Techniques (PETs) used in Privacy-Preserving Data Publishing (PPDP) using open-source libraries.
- Evaluate each technique's effectiveness in balancing privacy protection and data utility.
- Compare techniques using a common dataset and consistent utility/privacy metrics.

---

## 🔍 Techniques & Tools Used

| Technique                 | Library                          | Description |
|--------------------------|----------------------------------|-------------|
| Anonymization            | AnonyPy, Anjana                  | Applied k-anonymity using suppression and generalization. Utility measured by suppression level. |
| Synthetic Data Generation| SDV (GaussianCopula, CTGAN, TVAE)| Generated synthetic data. Evaluated with statistical distance and classification accuracy. |
| Differential Privacy     | Diffprivlib                      | Applied differentially private logistic regression using various epsilon values. Utility assessed by classification performance. |

---

## 📊 Dataset

- **UCI Adult Income Dataset** (Kaggle version - preprocessed):  
  [https://www.kaggle.com/datasets/uciml/adult-census-income](https://www.kaggle.com/datasets/uciml/adult-census-income)

---

## 📈 Results Summary

- **Anonymization**: Utility dropped as privacy levels increased. Suppression level rose with higher values of *k*. Anjana showed better utility preservation than AnonyPy.
- **Synthetic Data**: GaussianCopula was used as the main model. While privacy was preserved (as indicated by statistical distance), classification accuracy dropped by approximately 7%.
- **Differential Privacy**: Provided the best privacy-utility trade-off. Accuracy improved with higher epsilon values, with minimal gains beyond ε = 5.

---

## 📄 Report

The full internship report and presentation slides are available in the `report/` directory of this repository.

---

## 👩‍💻 Author

**Laurine Owino**  
Intern at Université de Sherbrooke  

---

## 🧩 Library Attribution

This project makes use of the following open-source libraries:

- **AnonyPy**   
  GitHub: [https://github.com/glassonion1/anonypy](https://github.com/glassonion1/anonypy)

- **Anjana**   
  GitHub: [https://github.com/IFCA-Advanced-Computing/anjana](https://github.com/IFCA-Advanced-Computing/anjana)

- **SDV (Synthetic Data Vault)**  
  GitHub: [https://github.com/sdv-dev/SDV](https://github.com/sdv-dev/SDV)

- ***DataSynthesizer**
  Github: [https://github.com/DataResponsibly/DataSynthesizer] (https://github.com/DataResponsibly/DataSynthesizer)

- **Diffprivlib (IBM Differential Privacy Library)**  
  GitHub: [https://github.com/IBM/differential-privacy-library](https://github.com/IBM/differential-privacy-library)

All libraries are used under their respective open-source licenses.

