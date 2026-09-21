# Single-Layer, Compact, High Isolation Dual-Band MIMO Antenna for WiFi 6/6E Applications

## 📄 Submission Information
- **Journal:** IEEE Latin America Transactions
- **Submission ID:** `10975`

---

## 👥 Authors & Affiliations

1. **Cuong Do-Manh** *(Corresponding Author)*  
   - Faculty of Electrical and Electronic Engineering, PHENIKAA School of Engineering, PHENIKAA University, Hanoi 12116, Vietnam  
   - Email: [cuong.domanh@phenikaa-uni.edu.vn](mailto:cuong.domanh@phenikaa-uni.edu.vn)

2. **Thao Hoang-Thi-Phuong**  
   - Faculty of Electronics and Telecommunications, Electric Power University, Hanoi, Vietnam  
   - Email: [thaohp@epu.edu.vn](mailto:thaohp@epu.edu.vn)

3. **Quyen Nguyen-Xuan**  
   - School of Electrical and Electronic Engineering, Hanoi University of Science and Technology (HUST), Hanoi, Vietnam  
   - Email: [quyen.nguyenxuan@hust.edu.vn](mailto:quyen.nguyenxuan@hust.edu.vn)

4. **Yem Vu-Van**  
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
| `Fig. 2 - S11.csv` & `Fig. 2 - Gain.csv` | Simulated reflection coefficient $|S_{11}|$ and peak realized gain of the single dual-band radiating element across 4.8–7.2 GHz. | Section II, Fig. 2 |
| `Fig. 3a.csv` & `Fig. 3b.csv` | Parametric study demonstrating independent frequency tuning by varying lower patch length $l_1$ and upper patch length $l_2$. | Section II, Fig. 3 |
| `Fig. 5.csv` | S-parameters ($|S_{11}|, |S_{21}|$) of the baseline MIMO antenna (MIMO-1) with identical element orientation. | Section III, Fig. 5 |
| `Fig. 6.csv` | S-parameters of MIMO-2 with inverted element configuration. | Section III, Fig. 6 |
| `Fig. 7.csv` | S-parameters of the final proposed MIMO-3 with inverted configuration and grounded decoupling stubs. | Section III, Fig. 7 |
| `Fig. 12 - *.csv` | Diversity performance evaluation metrics: ECC, MEG ($dB_{10}$), TARC ($dB_{20}$), and CCL. | Section IV-D, Fig. 12 |
| `Fig. 14a.csv` & `Fig. 14b.csv` | Comparison between simulated and measured S-parameters ($|S_{11}|, |S_{21}|$) and peak realized gain of the fabricated prototype. | Section V, Fig. 14 |
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


## 🔬 Fabrication & Experimental Verification

The physical prototype was fabricated on a $1.52\text{ mm}$ thick **Taconic RF-35** dielectric substrate ($\varepsilon_r = 3.5, \tan\delta = 0.0018$).
- **S-parameter measurement:** Measured using a calibrated Vector Network Analyzer (VNA).
- **Radiation patterns & gain:** Measured inside a standard far-field anechoic chamber.

| Parameter | Lower Band (Wi-Fi 6) | Upper Band (Wi-Fi 6E) |
| :--- | :--- | :--- |
| **Simulated Bandwidth ($|S_{11}| \le -10\text{ dB}$)** | 5.20 – 5.37 GHz (3.2%) | 6.60 – 6.80 GHz (3.0%) |
| **Measured Bandwidth ($|S_{11}| \le -10\text{ dB}$)** | 5.20 – 5.40 GHz (3.8%) | 6.60 – 6.84 GHz (3.6%) |
| **Inter-port Isolation ($|S_{21}|$ / $|S_{12}|$)** | $> 20\text{ dB}$ | $> 20\text{ dB}$ |
| **Measured Peak Realized Gain** | 4.6 – 5.0 dBi | 5.6 – 6.4 dBi |
| **Radiation Efficiency** | $\approx 94\%$ | $\approx 94\%$ |

---

## 🏛️ Acknowledgments

This research was funded and supported by the **Vietnam National Foundation for Science and Technology Development (NAFOSTED)** under Grant number **`102.04-2023.28`**.

---

## 📬 Contact & Inquiries

For technical questions or inquiries regarding the simulation model and measurement data, please contact:
- **Cuong Do-Manh** (Corresponding author): [cuong.domanh@phenikaa-uni.edu.vn](mailto:cuong.domanh@phenikaa-uni.edu.vn)
