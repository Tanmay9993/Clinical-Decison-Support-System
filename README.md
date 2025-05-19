# 🏥 Clinical Decision Support System (CDSS)

## 🔍 Overview
This project presents an intelligent Clinical Decision Support System that allows medical professionals and researchers to query patient records using natural language. Built on MIMIC-IV data, the system integrates structured hospital records into a semi-structured format, indexes them with LlamaIndex, and retrieves relevant patient insights using GPT-4—all through a user-friendly Streamlit interface.

## 🎯 Purpose & Problem Statement
Modern healthcare systems often suffer from data fragmentation, making it hard for clinicians to extract patient-level insights quickly. This project aims to streamline access to detailed patient histories—including admissions, medications, lab results, diagnoses, and procedures—by enabling AI-powered querying of rich longitudinal data to support better clinical decisions.

## 🛠️ Key Features & Workflow
- **Data Source**: MIMIC-IV database (PostgreSQL)
- **ETL & Preprocessing**:
  - Extracted core views (e.g., admissions, diagnoses, labs)
  - Transformed into a semi-structured hierarchical JSON format
  - Reduced JSON volume to enhance performance
- **AI & Indexing**:
  - Converted JSON data into structured clinical narratives
  - Used `LlamaIndex` + `OpenAI GPT-4` to create vector search index
  - Enabled natural language understanding for clinical questions
- **Frontend**:
  - Developed an interactive **Streamlit** app for clinicians
  - Accepts user queries and displays structured patient summaries
  - Includes patient navigation and visual theming

## 📈 Results & Visuals

### 🔹 Output Example 1:
<img width="1512" alt="UI-Output-1" src="https://github.com/user-attachments/assets/f99e4802-1d60-4ded-8ee6-5c74df237fd6" />

---

### 🔹 Output Example 2:
<img width="1512" alt="UI-Output-2" src="https://github.com/user-attachments/assets/a4b4a3d3-037a-40e0-a0e7-e0db211818f8" />

---


### 🔹 Output Example 3:
<img width="1511" alt="UI-Output-3" src="https://github.com/user-attachments/assets/19bc2a94-81af-473c-8b6b-9ee5ed1a110b" />

---

<br></br>

<h1>Data Source</h1> 
This project uses the [MIMIC-IV Clinical Database Demo (version 2.2)](https://physionet.org/content/mimic-iv-demo/2.2/).  

<h3>Database:</h3>
Johnson, A., Bulgarelli, L., Pollard, T., Horng, S., Celi, L. A., and Mark, R. (2023) 'MIMIC-IV Clinical Database Demo' (version 2.2), PhysioNet. 
Available at: https://doi.org/10.13026/dp1f-ex47.

<h3>Physionet</h3>
Goldberger, A., Amaral, L., Glass, L., Hausdorff, J., Ivanov, P.C., Mark, R., Mietus, J.E., Moody, G.B., Peng, C.K. and Stanley, H.E., 
2000. PhysioBank, PhysioToolkit, and PhysioNet: Components of a new research resource for complex physiologic signals. Circulation [Online]. 
101 (23), pp. e215–e220.
