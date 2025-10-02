# 🎓 QS World University Rankings – Web Scraping Project

## 📌 Overview
This project focuses on scraping data from the **QS World University Rankings** website to collect comprehensive information about universities worldwide.  

Since the dataset was too large to process in a single iteration, the scraping process was broken into **modular tasks**, with each module focusing on specific categories such as admissions, rankings, staff/student ratios, and locations.  

All extracted data is stored as **CSV files in well-organized folders**, making it easy to merge, analyze, and reuse.  

---

## 🗂 Project Structure

The repository is organized into multiple folders, each corresponding to a specific scraping task:

- **University Urls/**
  - Notebook: `UniversityUrls.ipynb`  
  - Extracts university names and URLs.  
  - Data split into 7 CSV files (`universities_with_no_100.csv` … `universities_with_no_700.csv`).  
  - Merged file: `UniversityUrls_Filesmerged_file.csv` (via `MergedCsvs.ipynb`).  

- **Admissions/**
  - Notebook: `admissions.ipynb`  
  - Extracts admission scores for courses.  
  - Data split into 7 CSV files (`university_admission_data1.csv` … `university_admission_data7.csv`).  
  - Merged file: `Admissions_Filesmerged_file.csv` (via `MergedCsvs.ipynb`).  

- **Students Staffs/**
  - Notebook: `StudentsStaffs.ipynb`  
  - Extracts student and staff counts.  
  - Data split into 7 CSV files (`studentstaff_count_1.csv` … `studentstaff_count_7.csv`).  
  - Merged file: `StudentsStaffs_Filesmerged_file.csv` (via `StudentsStaffs_Merge.ipynb`).  

- **Locations/**
  - Notebook: `Locations.ipynb`  
  - Extracts university location details (country, city, region).  
  - Data split into 7 CSV files (`university_locations_1.csv` … `university_locations_7.csv`).  
  - Merged file: `Locations_Filesmerged_file.csv` (via `Locations_Merge.ipynb`).  

- **Programs Available/**
  - Notebook: `ProgramsAvailable.ipynb`  
  - Extracts programs offered by universities.  
  - Data split into 7 CSV files (`programsavailable1.csv` … `programsavailable7.csv`).  
  - Merged file: `ProgramsAvailable_Filesmerged_file.csv` (via `ProgramsAvailable_Merge.ipynb`).  

- **Rankings/**
  - Notebook: `FinalRanks.ipynb`  
  - Extracts final ranking information.  
  - Data split into 7 CSV files (`FinalRankings1.csv` … `FinalRankings7.csv`).  
  - Merged file: `Rankings_Filesmerged_file.csv` (via `Rankings_Merge.ipynb`).  

- **Details/**
  - Notebook: `DetailsUniversity.ipynb`  
  - Extracts detailed information (University Name, Country, City, Region).  
  - CSV file: `details_universities.csv`  

⚠️ Currently limited to **1422 universities (2023 rankings)** due to kernel limitations on large-scale scraping.  

---

## ⚙️ Tech Stack
- **Language:** Python  
- **Libraries Used:**  
  - `BeautifulSoup` → for web scraping  
  - `Requests` → for HTTP requests  
  - `Pandas` → for data handling & CSV operations  
  - `Jupyter Notebook` → for code execution and modularity  

---

## 📊 Results
✅ Scraped and stored **structured datasets** covering:  
- University names & URLs  
- Admission scores  
- Student & staff counts  
- Locations (country, city, region)  
- Available programs  
- QS final rankings  
- Additional university details  

👉 The datasets are stored in **clean, merged CSV files** for easy downstream analysis and visualization.  

---

## 🔮 Future Enhancements
- Optimize scraping to handle **all universities** without kernel crashes.  
- Automate merging steps into a **single pipeline**.  
- Add **visualization notebooks** (charts, maps, trends).  
- Extend coverage to **multiple years** of QS rankings.  

---
