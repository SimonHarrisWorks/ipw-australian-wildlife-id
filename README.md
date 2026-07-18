# IPW Australian Wildlife Identification App
Offline wildlife identification prototype for 24 Australian species using **[EfficientNet‑B0](ca://s?q=Tell_me_more_about_EfficientNet_B0)**, **[PyTorch](ca://s?q=Tell_me_more_about_PyTorch)**, and **[Streamlit](ca://s?q=Tell_me_more_about_Streamlit)**. Includes GBIF species distribution maps, super‑species fallback logic, and downloadable Windows builds under Releases.

---

## Overview
IPW (Identify‑Per‑Wildlife) is a lightweight, offline wildlife recognition tool designed for conservation workflows.  
It identifies 24 Australian mammals and birds, provides confidence scores, assigns super‑species groups, and visualises species distribution using GBIF GeoJSON data.

This repository contains the full source code for review, along with two downloadable Windows builds under Releases.

---

## Features
- EfficientNet‑B0 image classification  
- 24 Australian species supported  
- Super‑species fallback when confidence is low  
- GBIF species distribution maps (GeoJSON)  
- Offline execution  
- Embedded Python runtime for portable builds  
- Streamlit interface  
- One‑click launch via `run.bat`

---

# Downloads (Releases)
Two builds are available under Releases.

## 1. Windows Portable Version  
**IPW‑Portable‑Windows.zip**

- No installation required  
- Includes embedded Python runtime  
- All dependencies bundled  
- Unzip and run `run.bat`

## 2. Standard Windows Build (Non‑Portable)  
**IPW‑Standard‑Windows.zip**

- Requires a local Python installation  
- Suitable for developers who want to modify or inspect the code  
- Run with:  
  ```
  streamlit run app.py
  ```

---

## Repository Contents
```
IPW-Python/                 # Embedded Python runtime
maps_csv/                   # CSV versions of species maps
app.py                      # Main Streamlit application
IPW.html                    # HTML export (not required for the app)
ipw_efficientnet_b0_best.pt # EfficientNet-B0 trained model weights
README.md                   # Project documentation
run.bat                     # Windows launcher for portable version
```

---

## Running the App (Developer Mode)
If running from source:

```
streamlit run app.py
```

Requires:
- Python 3.10+  
- PyTorch  
- Streamlit  
- Pillow  
- GeoPandas (optional for map processing)

---

## Species Included
24 species including:

- Bare‑nosed wombat  
- Southern hairy‑nosed wombat  
- Koala  
- Eastern grey kangaroo  
- Red kangaroo  
- Swamp wallaby  
- Common brushtail possum  
- Short‑beaked echidna  
- Additional species included in the model

---

## Future Work
- Mange detection module  
- CNN‑based health scoring  
- Burrow mapping integration  
- Routing for field surveys  
- Additional species  
- Mobile version

---

## License
This project is licensed under the MIT License.  
See the `LICENSE` file for details.

---

## Acknowledgements
- GBIF for species distribution data  
- PyTorch and EfficientNet authors  
- Streamlit for rapid prototyping  

