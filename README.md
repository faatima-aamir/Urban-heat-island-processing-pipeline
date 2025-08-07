# 🌡️ Urban Heat Island Detection Pipeline (South Asia)

This project automates the detection of Urban Heat Islands (UHI) across South Asia using MODIS satellite data (MOD11A2 – Land Surface Temperature). Developed in Jupyter Lab with Python, this notebook-based workflow includes automated data fetching, preprocessing, spatial clipping, LST computation, and UHI mapping.

---

## 🔧 Tools & Technologies

- **Platform**: Jupyter Lab (Anaconda)
- **Language**: Python
- **Data Source**: MODIS MOD11A2 (LST)
- **Libraries**:
  - `requests`, `os`, `datetime`
  - `rasterio`, `gdal`, `numpy`, `pandas`
  - `matplotlib`, `seaborn`, `geopandas`, `shapely`
  - `zipfile`, `glob`, `folium`

---

## ✨ Key Features

- Automates MODIS data download for specific tiles over Pakistan & South Asia
- Processes 8-day composite LST values for summer months (May–August)
- Clips imagery to urban boundaries using shapefiles
- Computes urban heat trends using mean, max, min temperatures
- Visualizes temperature maps and hotspot zones
- Saves outputs and graphs locally

---
## 🚀 How to Run

1. **Clone the Repository**  
git clone https://github.com/faatima-aamir/urban-heat-island-pipeline.git
cd urban-heat-island-pipeline
2. **Create & Activate Environment**
conda create -n uhi_env python=3.10
conda activate uhi_env
3. **Install Requirements**
pip install -r requirements.txt
4. **Launch Notebook**
jupyter lab
Run All Cells in processingpipeline_updated.ipynb

## 🚀 Output Images:
Monthly Mean:
<img width="1544" height="749" alt="image" src="https://github.com/user-attachments/assets/5f97c0ab-c400-433e-8ab5-8b7634d06483" />
Mosaicked LST with gradient color to show Land Surface Temperature:
<img width="1054" height="810" alt="image" src="https://github.com/user-attachments/assets/0a04968b-20c9-4d21-8dc1-93d94454cce1" />
Heat Map for year 2001:
<img width="577" height="358" alt="image" src="https://github.com/user-attachments/assets/b93d97ab-7718-449a-a346-cf0a09153791" />
Heat Map for 2002:
<img width="626" height="393" alt="image" src="https://github.com/user-attachments/assets/98435339-be14-48a5-b728-24dfc8cecdfd" />
Persistent and Transient Urban Heat Island Detection:
<img width="1345" height="628" alt="image" src="https://github.com/user-attachments/assets/ce3fa448-5ec4-4ae1-b154-3bc329acbe04" />
Rural and Urban UHI Zones Count:
<img width="809" height="606" alt="image" src="https://github.com/user-attachments/assets/b9b81ab0-be1f-4fc3-a63a-a80d972e2538" />

🙋‍♀️ Author
Faatima Aamir
www.linkedin.com/in/faatima-aamir-723a8b292



