# Single-Layer, Compact, High Isolation Dual-Band MIMO Antenna for WiFi 6/6E Applications

## 📄 Submission Information
- **Journal:** IEEE Latin America Transactions
- **Submission ID:** `10975`

---

## 👥 Authors & Affiliations

1. **Cuong Do-Manh**   
   - Faculty of Electrical and Electronic Engineering, PHENIKAA School of Engineering, PHENIKAA University, Hanoi 12116, Vietnam  
   - Email: [cuong.domanh@phenikaa-uni.edu.vn](mailto:cuong.domanh@phenikaa-uni.edu.vn)

2. **Thao Hoang-Thi-Phuong**  
   - Faculty of Electronics and Telecommunications, Electric Power University, Hanoi, Vietnam  
   - Email: [thaohp@epu.edu.vn](mailto:thaohp@epu.edu.vn)

3. **Quyen Nguyen-Xuan**  
   - School of Electrical and Electronic Engineering, Hanoi University of Science and Technology (HUST), Hanoi, Vietnam  
   - Email: [quyen.nguyenxuan@hust.edu.vn](mailto:quyen.nguyenxuan@hust.edu.vn)

4. **Yem Vu-Van** *(Corresponding Author)*
   - School of Electrical and Electronic Engineering, Hanoi University of Science and Technology (HUST), Hanoi, Vietnam  
   - Email: [yem.vuvan@hust.edu.vn](mailto:yem.vuvan@hust.edu.vn)

---

## 📖 About This Repository

This repository provides the official simulation models, numerical data, experimental measurement results, and manuscript files for the research paper:

> **"Single-Layer, Compact, High Isolation Dual-Band MIMO Antenna for WiFi 6/6E Applications"** (Submission ID: `10975`, *IEEE Latin America Transactions*).

### 🎯 Key Highlights of the Proposed Antenna
- **Single-layer planar profile:** Implemented on a single Taconic RF-35 substrate ($h = 1.52\text{ mm}$, $\varepsilon_r = 3.5$) without complex multilayer stacking or defected ground structures.
- **Dual-band capacitive excitation:** Independent control of the lower band (5.2–5.4 GHz, Wi-Fi 6) and upper band (6.60–6.84 GHz, Wi-Fi 6E) with low cross-sensitivity.
- **High isolation decoupling strategy:** Combines an inverted element arrangement (achieving $>20\text{ dB}$ isolation at the upper band) and grounded decoupling stubs (enhancing lower-band isolation to $>20\text{ dB}$).
- **Compact footprint:** Overall size of $0.61\lambda \times 0.61\lambda \times 0.03\lambda$ at 5.2 GHz with an edge-to-edge inter-element distance of only $d_e = 3\text{ mm}$ ($0.05\lambda$).
- **Excellent diversity metrics:** Low Envelope Correlation Coefficient ($\text{ECC} \approx 0$), balanced Mean Effective Gain ($\text{MEG} \approx -3\text{ dB}$), $\text{TARC} < -10\text{ dB}$, and Channel Capacity Loss ($\text{CCL} < 0.4\text{ bps/Hz}$).

---

## 📁 Repository Structure & File Descriptions

```text
.
├── LatinTrans - Nafosted Single Layer Dual band MIMO.pdf   # Accepted manuscript PDF
├── Simulation Files.aedt                                    # Ansys HFSS / Electronics Desktop simulation file
├── Figs. 1-4-8.txt                                          # Notes on extracting Figs. 1, 4, and 8 from AEDT
│
├── Fig. 2 - S11.csv                                         # Fig. 2: Simulated |S11| of the single dual-band element
├── Fig. 2 - Gain.csv                                        # Fig. 2: Simulated peak realized gain vs. frequency
├── Fig. 3a.csv                                              # Fig. 3a: Parametric sweep of patch length l1 on |S11|
├── Fig. 3b.csv                                              # Fig. 3b: Parametric sweep of patch length l2 on |S11|
├── Fig. 5.csv                                               # Fig. 5: Simulated S-parameters for MIMO-1 (co-directional)
├── Fig. 6.csv                                               # Fig. 6: Simulated S-parameters for MIMO-2 (inverted)
├── Fig. 7.csv                                               # Fig. 7: Simulated S-parameters for MIMO-3 (final design)
│
├── Fig. 9.csv                                               # Fig. 9: Parametric sweep of decoupling stub dimension bb on |S21|
├── Fig. 10.csv                                              # Fig. 10: Parametric sweep of stub parameter bb_c on |S21|
├── Fig. 11.csv                                              # Fig. 11: Parametric sweep of ground stub parameter gx1 on |S11|
│
├── Fig. 12 - ECC.csv                                        # Fig. 12a: Envelope Correlation Coefficient (ECC)
├── Fig. 12 - MEG.csv                                        # Fig. 12a: Mean Effective Gain (MEG1, MEG2)
├── Fig. 12 - TARC.csv                                       # Fig. 12b: Total Active Reflection Coefficient (TARC)
├── Fig. 12 - CHANNEL CAPACITY LOSS.csv                      # Fig. 12b: Channel Capacity Loss (CCL)
│
├── Fig. 14a.csv                                             # Fig. 14a: Simulated vs. measured S-parameters (|S11|, |S21|)
├── Fig. 14b.csv                                             # Fig. 14b: Simulated vs. measured peak realized gain
├── Fig. 15 - 5.3 GHz.csv                                    # Fig. 15: Radiation pattern data at 5.3 GHz (Phi/Theta cut)
└── Fig. 15 - 6.7 GHz.csv                                    # Fig. 15: Radiation pattern data at 6.7 GHz (Phi/Theta cut)
```

### 📝 Detailed Description of Files

| File Name | Description | Related Section / Figure in Paper |
| :--- | :--- | :--- |
| `LatinTrans - Nafosted Single Layer Dual band MIMO.pdf` | Full text manuscript formatted according to IEEE Latin America Transactions guidelines. | All Sections |
| `Simulation Files.aedt` | Complete 3D full-wave electromagnetic simulation model in **Ansys HFSS (Electronics Desktop)**, including 3D geometries, port definitions, boundary conditions, and frequency sweeps. | Sections II, III, IV, V |
| `Figs. 1-4-8.txt` | Explanatory note indicating that **Fig. 1** (Geometry & dimensions), **Fig. 4** (Design evolution), and **Fig. 8** (Surface current distributions at 5.2 GHz) are built directly inside `Simulation Files.aedt`. | Figs. 1, 4, 8 |
| `Fig. 2 - S11.csv` & `Fig. 2 - Gain.csv` | Simulated reflection coefficient $\vert S_{11}\vert$ and peak realized gain of the single dual-band radiating element across 4.8–7.2 GHz. | Section II, Fig. 2 |
| `Fig. 3a.csv` & `Fig. 3b.csv` | Parametric study demonstrating independent frequency tuning by varying lower patch length $l_1$ and upper patch length $l_2$. | Section II, Fig. 3 |
| `Fig. 5.csv` | S-parameters ($\vert S_{11}\vert, \vert S_{21}\vert$) of the baseline MIMO antenna (MIMO-1) with identical element orientation. | Section III, Fig. 5 |
| `Fig. 6.csv` | S-parameters of MIMO-2 with inverted element configuration. | Section III, Fig. 6 |
| `Fig. 7.csv` | S-parameters of the final proposed MIMO-3 with inverted configuration and grounded decoupling stubs. | Section III, Fig. 7 |
| `Fig. 9.csv` | Parametric sweep of decoupling stub dimension $b_b$ showing isolation improvement in $\vert S_{21}\vert$. | Section IV-B, Fig. 9 |
| `Fig. 10.csv` | Parametric sweep of stub position/clearance parameter $b_{bc}$ on inter-element isolation $\vert S_{21}\vert$. | Section IV-B, Fig. 10 |
| `Fig. 11.csv` | Parametric sweep of grounding stub parameter $g_{x1}$ demonstrating matching optimization on $\vert S_{11}\vert$. | Section IV-B, Fig. 11 |
| `Fig. 12 - *.csv` | Diversity performance evaluation metrics: ECC, MEG ($dB_{10}$), TARC ($dB_{20}$), and CCL. | Section IV-D, Fig. 12 |
| `Fig. 14a.csv` & `Fig. 14b.csv` | Comparison between simulated and measured S-parameters ($\vert S_{11}\vert, \vert S_{21}\vert$) and peak realized gain of the fabricated prototype. | Section V, Fig. 14 |
| `Fig. 15 - 5.3 GHz.csv` & `Fig. 15 - 6.7 GHz.csv` | 2D Radiation patterns (E-plane and H-plane / Co- and Cross-polarization) at 5.3 GHz and 6.7 GHz. | Section V, Fig. 15 |

---

## 🚀 How to Use the Provided Files

### 1. Opening and Running Full-Wave EM Simulations
1. Install **Ansys Electronics Desktop (HFSS)** (version 2021 R1 or newer recommended).
2. Open `Simulation Files.aedt` directly in Ansys Electronics Desktop.
3. In the Project Manager window:
   - **Antenna Geometries & Evolution (Figs. 1, 4):** Inspect the 3D solid model, parameterized dimensions (`Ls`, `lf`, `wf`, `df`, `s`, `s1`, `s2`, `l1`, `w1`, `l2`, `w2`, `ld`, `wd`, `rv`, `dv`, `g`), and substrate layers.
   - **Current Distributions (Fig. 8):** Right-click on `Field Overlays` $\rightarrow$ `Jsurf` to view surface current vectors and magnitudes on the patches and grounded stubs at 5.2 GHz and 6.7 GHz.
   - **S-parameters & Radiation Patterns:** Expand `Results` to re-plot or export S-parameters and Far Field Gain plots.

---

### 2. Plotting and Analyzing CSV Data

The provided `.csv` files can be processed and visualized using **Python**, **MATLAB**, or **OriginPro**.

#### Quick Visualization with Python:

Ensure you have `matplotlib` and `pandas` installed:
```bash
pip install pandas matplotlib
```

Run the following Python script to plot the S-parameters (Fig. 14a) and peak gain (Fig. 14b):

```python
import pandas as pd
import matplotlib.pyplot as plt

# 1. Plot S-parameters (Fig. 14a)
df_s = pd.read_csv('Fig. 14a.csv')
plt.figure(figsize=(8, 5))
plt.plot(df_s['Freq [GHz]'], df_s['dB(S(1,1)) []'], label='|S11|', color='blue', linewidth=2)
plt.plot(df_s['Freq [GHz]'], df_s['dB(S(2,1)) []'], label='|S21|', color='red', linestyle='--', linewidth=2)
plt.axhline(-10, color='gray', linestyle=':', label='-10 dB threshold')
plt.axhline(-20, color='black', linestyle=':', label='-20 dB isolation')
plt.title('S-Parameters of Proposed MIMO Antenna (Fig. 14a)', fontsize=13)
plt.xlabel('Frequency (GHz)', fontsize=11)
plt.ylabel('Magnitude (dB)', fontsize=11)
plt.xlim([4.8, 7.2])
plt.ylim([-35, 0])
plt.grid(True, linestyle='--', alpha=0.6)
plt.legend(loc='lower right')
plt.tight_layout()
plt.show()

# 2. Plot MIMO Diversity Metrics (Fig. 12)
df_ecc = pd.read_csv('Fig. 12 - ECC.csv')
df_ccl = pd.read_csv('Fig. 12 - CHANNEL CAPACITY LOSS.csv')

fig, ax1 = plt.subplots(figsize=(8, 5))
ax1.plot(df_ecc['Freq [GHz]'], df_ecc['ECC []'], color='purple', linewidth=2, label='ECC')
ax1.set_xlabel('Frequency (GHz)', fontsize=11)
ax1.set_ylabel('ECC', color='purple', fontsize=11)
ax1.set_ylim([0, 0.5])
ax1.grid(True, linestyle='--', alpha=0.6)

ax2 = ax1.twinx()
ax2.plot(df_ccl['Freq [GHz]'], df_ccl['mag(CCL) []'], color='green', linestyle='--', linewidth=2, label='CCL (bps/Hz)')
ax2.set_ylabel('CCL (bps/Hz)', color='green', fontsize=11)
ax2.set_ylim([0, 0.5])

plt.title('MIMO Diversity Performance: ECC & CCL (Fig. 12)', fontsize=13)
fig.tight_layout()
plt.show()
```

#### In MATLAB:
```matlab
% Load and plot S-parameters
data = readmatrix('Fig. 14a.csv');
freq = data(:, 1);
s11  = data(:, 2);
s21  = data(:, 3);

figure;
plot(freq, s11, 'b-', 'LineWidth', 1.5); hold on;
plot(freq, s21, 'r--', 'LineWidth', 1.5);
yline(-10, 'k:'); yline(-20, 'm:');
xlabel('Frequency (GHz)');
ylabel('Magnitude (dB)');
title('S-Parameters of Proposed MIMO Antenna');
legend('|S_{11}|', '|S_{21}|', 'Threshold -10 dB', 'Isolation -20 dB');
grid on;
```

---

## 🔬 Fabrication & Experimental Verification

The physical prototype was fabricated on a $1.52\text{ mm}$ thick **Taconic RF-35** dielectric substrate ($\varepsilon_r = 3.5, \tan\delta = 0.0018$).
- **S-parameter measurement:** Measured using a calibrated Vector Network Analyzer (VNA).
- **Radiation patterns & gain:** Measured inside a standard far-field anechoic chamber.

| Parameter | Lower Band (Wi-Fi 6) | Upper Band (Wi-Fi 6E) |
| :--- | :--- | :--- |
| **Simulated Bandwidth ($\vert S_{11}\vert \le -10\text{ dB}$)** | 5.20 – 5.37 GHz (3.2%) | 6.60 – 6.80 GHz (3.0%) |
| **Measured Bandwidth ($\vert S_{11}\vert \le -10\text{ dB}$)** | 5.20 – 5.40 GHz (3.8%) | 6.60 – 6.84 GHz (3.6%) |
| **Inter-port Isolation ($\vert S_{21}\vert \text{ / } \vert S_{12}\vert$)** | $> 20\text{ dB}$ | $> 20\text{ dB}$ |
| **Measured Peak Realized Gain** | 4.6 – 5.0 dBi | 5.6 – 6.4 dBi |
| **Radiation Efficiency** | $\approx 94\%$ | $\approx 94\%$ |

---

## 📚 Citation

If you use these simulation models, datasets, or designs in your research, please cite our paper:

```bibtex
@article{domanh2026singlelayer,
  title={Single-Layer, Compact, High Isolation Dual-Band MIMO Antenna for WiFi 6/6E Applications},
  author={Do-Manh, Cuong and Hoang-Thi-Phuong, Thao and Nguyen-Xuan, Quyen and Vu-Van, Yem},
  journal={IEEE Latin America Transactions},
  note={Submission ID: 10975},
  year={2026}
}
```

---

## 🏛️ Acknowledgments

This research was funded and supported by the **Vietnam National Foundation for Science and Technology Development (NAFOSTED)** under Grant number **`102.04-2023.28`**.

---

## 📬 Contact & Inquiries

For technical questions or inquiries regarding the simulation model and measurement data, please contact:
- **Cuong Do-Manh** (Corresponding author): [cuong.domanh@phenikaa-uni.edu.vn](mailto:cuong.domanh@phenikaa-uni.edu.vn)
