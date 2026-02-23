# Benzene Exposure Estimation Tool

This Python-based tool estimates indoor benzene concentrations during gas stove use using a simple box model.  
It is part of **CIVE 442 – Exposure Estimation & Reasoning Tool**.

---

## 💡 How It Works
The model uses a mass-balance approach:

dC/dt = (E/V) - (Q/V) * C

where  
- **E** = emission rate (mg/min)  
- **V** = kitchen volume (m³)  
- **Q** = ventilation flow rate (m³/min) = (ACH × V) / 60

Concentration builds up while cooking and decays afterward.  
Outputs include:
- Peak benzene concentration (mg/m³)  
- Time-integrated exposure (mg·h/m³)  
- A plot of concentration vs. time

---

## ⚙️ Requirements
You can run this tool in any Python environment or directly in [Google Colab](https://colab.research.google.com/).

Modules used:
```bash
pip install matplotlib
