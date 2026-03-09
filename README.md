readme = """# Climate Change Analysis

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![License](https://img.shields.io/badge/License-MIT-green)

Uçtan uca iklim veri analizi: NASA GISTEMP ve Berkeley Earth verileriyle küresel ve Türkiye'ye özgü sıcaklık trendleri.

---

## About

This project analyzes global and Turkey-specific temperature trends using NASA GISTEMP and Berkeley Earth datasets. It includes data cleaning, time series visualization, and anomaly analysis covering 1750 to present.

---

## Project Structure
```
climate-analysis/
│
├── data:/                              # Raw datasets
│   ├── GlobalTemperatures.csv         # Berkeley Earth global temps
│   ├── GlobalLandTemperaturesByCountry.csv
│   └── gistemp250_GHCNv4.nc          # NASA NetCDF data
│
├── notebook.ipynb                     # Main analysis notebook
├── requirements.txt                   # Dependencies
└── README.md
```

---

## Data Sources

| Source | Dataset | Coverage |
|--------|---------|----------|
| NASA GISTEMP v4 | Global surface temperature anomalies | 1880–present |
| Berkeley Earth | Land temperatures by country | 1743–present |
| NOAA | Atmospheric CO2 (Mauna Loa) | 1958–present |

---

## Key Findings

- Global land surface temperature has increased significantly since the 1900s
- Turkey follows the global warming trend with a sharp rise after 2000
- Both global and Turkey anomalies show parallel trends since the industrial era

---

## Methods

- Time series analysis with 10-year rolling averages
- Temperature anomaly calculation (base period: 1951–1980)
- Global vs Turkey comparative visualization
- NetCDF file processing with xarray

---

## Installation
```bash
git clone https://github.com/YOUR_USERNAME/climate-analysis.git
cd climate-analysis
pip install -r requirements.txt
```

Open `notebook.ipynb` in Jupyter and run all cells.

---

## Libraries Used

- **pandas** — data manipulation
- **matplotlib** — visualization
- **xarray** — NetCDF processing
- **numpy** — numerical operations

---

## License

This project is licensed under the MIT License.

---

# İklim Değişikliği Analizi

NASA GISTEMP ve Berkeley Earth veri setleri kullanılarak 1750'den günümüze küresel ve Türkiye sıcaklık trendlerinin analizi.

## Temel Bulgular

- Küresel kara yüzeyi sıcaklığı 1900'lerden itibaren belirgin şekilde artmıştır
- Türkiye küresel ısınma trendini takip etmekte, 2000 sonrası keskin artış görülmektedir
- Her iki trend sanayi döneminden bu yana paralel seyretmektedir
"""

with open("README.md", "w") as f:
    f.write(readme)



