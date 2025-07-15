# 🌍 Landslide Prediction Using Tree-Based Models

A data science competition project from Virginia Tech that uses spatial and environmental data to predict the region where a rainfall-triggered landslide is likely to occur. Built using decision tree-based machine learning models.

---

## 🧪 Research Question

**In which region did a landslide occur given environmental conditions and specifications of the landslide?**

The goal is to use features such as rainfall, location, and date to accurately classify landslide occurrences into distinct regions of risk.

---

## 📊 Dataset

- **Name**: Global Landslide Catalog (GLC)
- **Source**: [NASA Open Data Portal](https://data.nasa.gov/Earth-Science/Global-Landslide-Catalog-Not-updated-/h9d8-neg4)
- **Years Covered**: 2007–2015
- **Size**: 6,788 rows × 35 columns
- **Purpose**: Identify rainfall-triggered landslides worldwide

[Direct CSV Download](https://data.nasa.gov/api/views/9ns5-uuif/rows.csv?date=20241116&accessType=DOWNLOAD)

---

## 🧠 Models Used

### 🌳 Random Forest
- Achieved **68.5% accuracy** on test data
- Hyperparameters: `ntree = 300`, `mtry = 18`
- Further tuning did not yield significant improvement

### ⚡ XGBoost
- Achieved **69.5% accuracy** without hyperparameter tuning
- Observed lower training error (0.02), but potential overfitting

---

## 📌 Region Definition

- Landslide regions were defined using a **100-mile radius** around events
- Formed clusters with at least 5 observations
- **86 distinct regions** were identified as classification targets

---

## 📈 Time Analysis

- Most landslides occurred in **July and August**
- Contrast with expected months like March and April
- **Training Data**: 2007–2012 (4,138 observations)  
- **Testing Data**: 2012–2015 (2,644 observations)

---

## 🛠️ Why Tree-Based Models?

- Handle both **discrete and continuous variables**
- Perform well with **high-dimensional spatial data** (e.g., latitude and longitude)
- More robust against noise and overfitting compared to linear models

---

## 📚 References

1. [USGS: What is a landslide and what causes one?](https://www.usgs.gov/faqs/what-a-landslide-and-what-causes-one)  
2. [NASA: Global Landslide Catalog](https://gpm.nasa.gov/landslides/about.html)

---

## 👥 Team

**Hokie Hackers** — Virginia Tech  
- Ted Li  
- Devanshu Khadka  
- Drew Keely  
- Nami Jain

---

## 📫 Contact

**Devanshu Khadka**  
[LinkedIn](https://linkedin.com/in/devanshukhadka)  
📧 khadkadevanshu@gmail.com

---

## 📜 License

For academic use only. Contact authors for reuse or collaboration.
