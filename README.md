
---

## Model Architecture

The hybrid model utilizes both sequential and spatial feature learning:

- **LSTM (Long Short-Term Memory)** to capture sequential patterns in features  
- **1D CNN (Convolutional Neural Networks)** to extract spatial correlations  
- **Dense Layers** for final classification  

This combination improves detection accuracy and minimizes false positives.

---

## Dataset Overview

The dataset contains **90 engineered features** extracted from URLs. These include:

- URL structure elements (length, special characters)
- Domain and subdomain info
- HTML/JS behaviors (like iframe, onmouseover, etc.)
- WHOIS and DNS metadata

Full feature descriptions are documented in:  
[`Phishing Features Doc.pdf`](./Phishing%20Features%20Doc.pdf)

The `label` column indicates:
- `0`: Legitimate  
- `1`: Phishing  

---

## Getting Started

### Install Dependencies

Ensure Python ≥3.7 is installed. Then:

```bash
pip install -r requirements.txt
