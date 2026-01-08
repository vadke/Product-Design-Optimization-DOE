# 🏎️ Product Design Optimization using DOE (Design of Experiments)

## 📌 Business Overview
In manufacturing and R&D, identifying the optimal combination of design inputs to maximize performance while minimizing cost is critical. This project utilizes **Design of Experiments (DOE)** to statistically analyze the factors affecting the performance (distance traveled) of a prototype vehicle.

## 📊 Methodology
We employed a **2⁴ Full Factorial Design** to test 4 design parameters across 16 unique configurations (with 3 replicates each for statistical validity).

* **Objective:** Maximize Distance Traveled ($Y$) subject to Cost Constraints.
* **Factors Tested ($X$):**
    1.  **Length:** (Big vs. Small)
    2.  **Load Distribution:** (Front vs. Back)
    3.  **Width:** (Large vs. Small)
    4.  **Tyre Size:** (Big vs. Small)
* **Sample Size:** 48 total runs (randomized order to eliminate bias).

  <img width="1150" height="586" alt="image" src="https://github.com/user-attachments/assets/ea2bf869-76bb-4be2-8a5b-330eff8afbe9" />


## 📈 Key Findings (ANOVA Analysis)
1.  **Main Effects:**
    * **Width** was the most significant factor; a "Large" width increased stability and distance.
    * **Length** had a strong positive correlation with performance.

    <img width="768" height="328" alt="image" src="https://github.com/user-attachments/assets/8b668b79-982d-4b3d-8cec-dcf40349ada1" />

2.  **Interaction Effects:**
    * A significant interaction was found between **Length** and **Width**. Increasing both simultaneously yielded exponential gains compared to increasing them individually.

    
    <img width="796" height="531" alt="image" src="https://github.com/user-attachments/assets/1f6298d8-48b5-4a2b-91c6-7c2b465888fd" />

3.  **Optimal Configuration:**
    * **Design:** Big Length + Back Load + Large Width + Small Tyres.
    * **Result:** Max Distance of **151.33 cm**.
    * **Cost Efficiency:** "Small Tyres" provided similar performance to "Big Tyres" but at a significantly lower cost, improving the margin.

<img width="1178" height="224" alt="image" src="https://github.com/user-attachments/assets/2c39e5a8-b189-4dfb-bff6-191df6059a8f" />

## 🛠 Tools Used
* **Statistical Software:** Minitab (ANOVA, Pareto Charts, Interaction Plots)
* **Data Collection:** Physical prototyping & Randomized trials
* **Analysis:** Regression Analysis, Residual Analysis (Normality/Homoscedasticity checks)

## 📂 Project Structure
* `M6 Lego Presentation.pptx` - Full report with Pareto Charts and Interaction Plots.
* `Minitab_Lego_Project.mpx` - Raw Minitab project file.
* `experiment_data.csv` - Raw experimental data.
