# **IRS-Assisted OFDM Communication System**

### **Overview**
This repository contains the implementation of an Intelligent Reflecting Surface (IRS)-assisted Orthogonal Frequency Division Multiplexing (OFDM) communication system. The project explores multi-user mobility patterns and their impact on spectral efficiency and bit-error rate (BER). It includes detailed simulations of user mobility using linear and 2D random walk models, equalization techniques, and IRS integration for enhanced signal strength and coverage.


### **Features**
- Simulates an OFDM transceiver with Rayleigh fading and IRS integration.
- Models user mobility with linear and 2D random walks.
- Implements modulation schemes like BPSK, QPSK, and 16QAM for BER vs. SNR analysis.
- Incorporates Long Short-Term Memory (LSTM) networks for user mobility prediction.
- Provides insights into IRS grid size, proximity effects, and multi-user scenarios.

---

### **Requirements**
- Python 3.8 or above
- Libraries: `numpy`, `matplotlib`, `scipy`, `tensorflow`, `sklearn`, `jupyter`

Install dependencies using:
```bash
pip install -r requirements.txt
```


### **How to Run**
1. Clone the repository:
   ```bash
   git clone https://github.com/YourUsername/IRS_OFDM_Project.git
   cd IRS_OFDM_Project
   ```
2. Set up a Python environment and install dependencies.
3. Run the Jupyter Notebooks in `/notebooks` for simulation:
   ```bash
   jupyter notebook
   ```
4. Alternatively, execute Python scripts in `/src` for specific modules:
   ```bash
   python src/ofdm_transceiver.py
   ```
---

### **Key Results**
1. **BER vs. SNR Analysis:**
   - BPSK provides better BER performance than QPSK and 16QAM.
   - Increasing IRS grid size improves signal quality marginally for static users.
   ![BER vs SNR](images/ber_vs_snr.png)

2. **Spectral Efficiency with User Mobility:**
   - Spectral efficiency peaks near the IRS and decreases with distance.
   - LSTM predictions smoothen mobility simulation results.
   ![Spectral Efficiency](images/spectral_efficiency.png)

3. **Multi-User Scenario:**
   - Sum rates increase exponentially with SNR in multi-user simulations.

---

### **References**
- Wu, Q., Zhang, S., Zheng, B., You, C., & Zhang, R. (2021). "Intelligent Reflecting Surface-Aided Wireless Communications: A Tutorial." *IEEE Transactions on Communications.*
- Ahmed, Q. (2023). "BER Analysis of IRS-Assisted Wireless Communications in Generalized Gaussian Noise." *IEEE Transactions on Vehicular Technology.*
