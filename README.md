# nasa-planet-hunter
A machine learning project that detects exoplanets using NASA Kepler data.

### Mission overview
Nasa's KELPER telescope observed over 9000 stars during its time, flagging them as 'candidates'. My goal was to build a machine learning model to differenciate real exo planets, to junk/false positives automatically

### Tech Stack
# Language: Python 3
# Librarys: Panda, Scikit-Learn, Matplotlib, Numpy
# Random Forest Classifier (Optimized via Grid Search)

### Key Results
* **Accuracy:** ~92% on unseen test data.
* **Insight:** The model identified **Planet Radius (`koi_prad`)** as the single most critical feature for determining planetary status, aligning with astrophysical theory.
* **Optimization:** Tuned hyperparameters (200 Trees, Max Depth 20) to balance Precision and Recall.

###  How It Works
1.  **Data Cleaning:** Filtered raw NASA data to remove noisy labels.
2.  **Training:** Used a Random Forest algorithm to learn patterns from 80% of the dataset.
3.  **Validation:** Tested the remaining 20% to generate a Confusion Matrix.
4.  **Tuning:** Reduced the probability threshold to 0.20 to aggressively hunt for rare Earth-like planets (minimizing False Negatives).

---
*Created by Enzo Leite Sanches*

