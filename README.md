# **<p align="center">MechaCar Analysis</p>**

### **<p align="center">A statistical analysis of AutosRUs’ newest prototype, the MechaCar.</p>**

---
## Linear Regression to Predict MPG
---

<p align="center">
   <img width="700" height="450" src="https://github.com/Jamesrx33/MechaCar_Statistical_Analysis/blob/main/Resources/Images/Linear%20Regression%20Summary.png?raw=true">
</p>

* Vehicle Length and Ground Clearance attributed to a non-random amount of variance
* The slope of this linear model is **not** considered to be zero due to a very low p-value of 5.35e-11
* With a multiple R-Squared value of .71, this model has a strong Pearson's correlation and predicts the MechaCar Prototype's MPG effectively

---
## Summary Statistics on Suspension Coils
---

<p align="center">
<img src="https://github.com/Jamesrx33/MechaCar_Statistical_Analysis/blob/main/Resources/Images/PSI_Summary_Stats.png?raw=true">
</p>

* The total summary of PSI data falls within the acceptable limits of variance
  > 62.3 is less than the maximum allowed variance of 100
* Lots 1 and 2 have very low variance with consistent Means and Medians
* Lot 3 has a deviating Mean and Median and its level of variance and fails to meet design specifications
  > A variance of ~170 exceeds the maximum of 100

---
## T-Tests on Suspension Coils
---

**Total Results**

<p align="center">
<img src="https://github.com/Jamesrx33/MechaCar_Statistical_Analysis/blob/main/Resources/Images/Total_t-test.png?raw=true">
</p>

**Lot 1**

<p align="center">
<img src="https://github.com/Jamesrx33/MechaCar_Statistical_Analysis/blob/main/Resources/Images/Lot1_t-test.png?raw=true">
</p>

**Lot 2**

<p align="center">
<img src="https://github.com/Jamesrx33/MechaCar_Statistical_Analysis/blob/main/Resources/Images/Lot2_t-test.png?raw=true">
</p>

**Lot 3**

<p align="center">
<img src="https://github.com/Jamesrx33/MechaCar_Statistical_Analysis/blob/main/Resources/Images/Lot3_t-test.png?raw=true">
</p>

* Taken as a whole, there is no statistical difference between the presumed population mean of 1500PSI and the observed data
* However, considering each lot individually, there is a statistical difference between the presumed and observed PSI Mean from Lot 3 -- its p-value of .04 is under the signifcance level of .05

---
## Study Design: MechaCar vs Competition
---

**City MPG One Sample T-Test**
In order to compare how the MechaCar performs vs other cars of the same class, we propose a One Sample T-Test given the following design:

1. We have a dataset of at least 500 cars from 20 or more different manufacturers
   * Each car in the dataset must be of the same "class" of car
     > Ex: "Sedan", "Truck", "SUV"...etc
   * The Mean City MPG is recorded daily for each car over 30 days
2. MechaCar data will be extracted as a sample and the Mean of the 30 days of City MPG recording will be tested against the population mean
3. Our Hypothesis:
   * **Null:** The mean City MPG of the MechaCar over 30 days is not different than the population mean
   * **Alternative:** The Mean City MPG of the MechaCar over 30 days is *greater* than the population mean
4. A right-tailed One Sample T-Test will be used to test this hypothesis
   * We chose this test because this is one sample taken from a population
   * The test is right-tailed because we are testing to see if mean MechaCar performance is more than 3 SD greater than the population mean
   * Rejecting the Null Hypothesis would show **MechaCar City MPG performance exceeds that of its competition**

---

## Reference Documentation - [Source Code Repository](https://github.com/Jamesrx33/MechaCar_Statistical_Analysis), [Download .zip file](https://github.com/Jamesrx33/MechaCar_Statistical_Analysis/archive/refs/heads/main.zip)
