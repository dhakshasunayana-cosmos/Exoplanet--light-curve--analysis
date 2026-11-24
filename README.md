# 🪐 Exoplanet Transit Light Curve Analysis: WASP-19b

An end-to-end astrophysics data analysis pipeline built in Python using NASA's TESS space telescope observations to detect and characterize the ultra-short-period hot Jupiter **WASP-19b**.

## 🔬 Key Findings
* **Target Star:** WASP-19 (TIC 35516889)
* **Detected Orbital Period:** `0.7888 days` (~18.9 hours)
* **Orbital Distance:** `~0.016 AU` (~60x closer to its host star than Earth is to the Sun)
* **Calculated Planet Radius:** `~1.3–1.4 R_Jup` (using custom transit-masked detrending to prevent flux dilution)

## 🛠️ Tools & Methodology
* **Data Ingestion:** `lightkurve` & `astropy` (MAST / TESS SPOC light curves)
* **Signal Processing:** Savitzky-Golay detrending with custom phase-based transit masking & sigma-clipping outlier removal
* **Transit Detection:** Box Least Squares (BLS) periodogram & phase-folding
