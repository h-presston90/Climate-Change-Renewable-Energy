# Overlooked Climate Risks: Performance Degradation and Correction of Renewable Energy Assessments under a Changing Climate

## 📘 Project Overview
This repository contains the implementation for the project titled **"Overlooked Climate Risks: Performance Degradation and Correction of Renewable Energy Assessments under a Changing Climate,"** developed as part of the **2025 CAE Internship Program**.


## 🚀 Getting Started

To begin using this repository for the first time:

1. Please refer to the **GitHub tools** section under *Other Resources*.
2. Clone this repository to your local machine.
3. All progress and development must be conducted **within this repository**.


## 🔄 Commit & Push Policy

- Regularly commit and push changes (recommended **daily**).
- Before each **weekly meeting**, you must:
  - Push your latest progress by **23:59 of the previous day**
  - Update the **progress report file** and your **weekly journal** (see the `weekly_meeting/` folder for reference)

## 🧑‍💻 Code
*To be developed. Below is the template.*

This project will include a modular and well-structured codebase, organized into the following components:

### 📁 Folder Structure (Planned)

```
src/
├── data_processing/       # Scripts for loading, cleaning, and transforming raw datasets
├── modeling/              # Optimization, forecasting, and simulation models
├── evaluation/            # Evaluation metrics and benchmarking tools
├── visualization/         # Plotting and visualization scripts
├── utils/                 # General-purpose helper functions
└── config/                # Configuration files (e.g., paths, parameters)
```

### 🧩 Planned Functional Modules

- **Data Preprocessing**
  - Parsing Taipower and ERA5 data
  - Time alignment and gap filling
  - Aggregation to hourly resolution

- **Stochastic Optimization**
  - Demand-side response modeling
  - Green electricity trading with uncertainty handling

- **Evaluation**
  - Cost-benefit analysis
  - Emission impact estimation
  - Visual comparisons and dashboards

- **Visualization**
  - Load and generation trends
  - Flow maps and marginal emission heatmaps

> 📌 Each module will include example usage in `notebooks/` and be designed for reproducibility.


## 📊 Data

### ✅ Available

- **`power_generation`**  
  2022 Unit-Level Power Generation Data (10-minute resolution)  
  Source: [Power Generation by Units – data.gov.tw](https://data.gov.tw/dataset/37331)  
  > 資料為2022年各發電機組的淨發電量，時間解析度為10分鐘

### 🔄 To Be Integrated

- **ERA5 hourly data on single levels (1940–present)**  
  Source: [ERA5 Reanalysis Dataset – Copernicus Climate Data Store](https://cds.climate.copernicus.eu/datasets/reanalysis-era5-single-levels?tab=overview)  
  > ERA5單層面氣象資料（每小時解析度）

- **CODiS Observational Climate Data (Taiwan)**  
  Source: [CODiS Platform – Central Weather Administration](https://codis.cwa.gov.tw)  
  > 中央氣象署觀測氣候資料，每小時解析度

---

## 📚 Literature

### 🔑 Key Reference

- **Projected patterns of climate change impact on photovoltaic energy potential A case study of Iraq**  
  > 關鍵文獻

---

## 🔗 Other Resources (Mandatory Reading)

- **GitHub Tools**  
  - [GitHub Desktop](https://desktop.github.com/download/) (**recommended**) [(教學影片)](https://www.youtube.com/watch?v=iJXreJ3XhZY&list=PLwE9aC2NIkXl7r6p5TtYlgKhCuzbB16OO&index=6)
  - [Git](https://git-scm.com/) (CLI)
  > 版本追縱工具
---

## 📖 Recommended Learning Materials
- **E3 Pi Day Workshop**  
  Academic sharing sessions presented by E3 members  
  Access the full playlist here: [YouTube](https://www.youtube.com/playlist?list=PLwE9aC2NIkXl7r6p5TtYlgKhCuzbB16OO)
  > 研究技巧分享，來自E3成員



- **Engineering Research Methods (113-2)**  
  Course Slides by Prof. Wang & Prof. Tsai  
  Access: [Google Drive Folder](https://drive.google.com/drive/folders/1JO1s7RvkZt7yfIl7uBJmadE-ceetQ5X3?usp=sharing)  
  > 研究方法介紹，來自工程科學研究方法課程

---
