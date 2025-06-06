# H–O–H Angle Deformation in Water: Energy Profile

This project investigates how the potential energy of a single water molecule changes with variations in the **H–O–H bond angle**. Using **Density Functional Theory (DFT)** calculations performed in ORCA, single-point energies were computed across a range of fixed angles to generate a detailed **energy profile** of angular deformation.

---

## Optimized Structure

The image below shows the geometry of a single water molecule used in this study:

![Optimized Water](./water.jpg)

---

## Methodology

- **System**: Single H₂O molecule  
- **Software**: ORCA for quantum chemistry; Python (Google Colab) for analysis  
- **Procedure**:
  - Begin from the optimized geometry of H₂O (equilibrium H–O–H angle ≈ 105.2°)
  - Fix O–H bond lengths and vary the **H–O–H bond angle** from 60° to 180° in 0.1° steps
  - Perform **single-point energy calculations** at each angle
  - Visualize and fit the energy curve using python.
 
---

## Input/Output Files
Over 300 ORCA input/output files were generated by scanning the H–O–H bond angle.

To explore a sample configuration:

🔹 Input:  [angle_water.inp](./H2O_angle_0096p6.inp)  
🔹 Output: [angle_water.out](./H2O_angle_0096p6.out)


---

## H–O–H Angle Energy Profile

This figure illustrates how the energy of a water molecule changes with angle deformation:

**visualize or download** the raw data used: [angle_energy_data.csv](./angle_energy_data.csv)

![H–O–H Energy Curve](./energy_curve.png)

---

**Interaction Behavior**:
- **Repulsion**: Angle = 60° → High energy due to strong steric repulsion  
- **Equilibrium**: Angle ≈ 105.2° → Minimum energy configuration  
- **Deformation**: Angle = 180° → Higher energy due to orbital strain  

---

## Energy Curve Fitting and Force Constant

To quantify the stiffness of **the H–O–H angle** in a water molecule, we performed a parabolic fit around the energy minimum.


**visualize or download** the raw data used: [View notebook: Angle_forceconst.ipynb](./Angle_forceconst.ipynb)
 

## A zoomed-in plot near the energy minimum 
![Parabolic Fit (near minimum)](./Parabolic_fits_near_minimum.png)

---

## Author

Created by: **Handson Gisubizo**  
 GitHub: [https://github.com/handsongisubizo](https://github.com/handsongisubizo)
