# HPE_TASKS
# 5G NR Configuration Data Extraction Project

**Project Overview**

This project focuses on the extraction of relevant 5G NR (New Radio) configuration data from XML files. It includes two main tasks:

- **Task 1:** Extract specific configuration details such as gNB ID, sector details, bandwidth, and frequency.
- **Task 2:** Extract neighbour cell information including home cell and associated neighbouring cells.

The extracted information is structured and exported to CSV format for analysis and further telecom network optimization.


## File Structure

| File Name                             | Description |
|-----------------------------------    |-------------|
| `Task1_Extract_Details.py`            | Python script for extracting detailed 5G NR configuration from XML. |
| `Task1_Report.docx`                   | Report summarizing Task 1 methodology, tools used, and output. |
| `Task2_Neighbour_cells.py`            | Python script for parsing and extracting neighbour cell data. |
| `Task2_Report.docx`                   | Report documenting Task 2's logic, output, and findings. |
| `ericsson_5g_cells.csv`               | output XML-converted CSV for Task 1. |
| `output_5g_cells_neighbour_cells.csv` | Output CSV from Task 2 containing neighbour cell mappings. |


## Task Descriptions

### Task 1: Extract Configuration Details

- Extracted elements include:
  - `gNB ID`
  - `Sector Equipment`
  - `Bandwidth`
  - `Frequency`
- The goal is to understand and structure the configuration of 5G cells.

### Task 2: Extract Neighbour Cell Mapping

- Extracted elements include:
  - `Home gNB`
  - `gNB Name`
  - `Home Cell`
  - `Neighbour Cell Info`
- This data is essential for optimizing handover and coverage planning.


## 🛠️ Technologies Used

- **Python 3.x**
- **pandas** – For tabular data handling and CSV generation
- **xml.etree.ElementTree** – For XML parsing
- **Microsoft Excel** – For visualization and validation of CSV output


## Output

- Task 1 Output: `ericsson_5g_cells.csv`
- Task 2 Output: `output_5g_cells_neighbour_cells.csv`
- These files can be directly opened in Excel or fed into network tools.



##  Reports

Each task has a detailed Word report explaining:
- Objectives
- Tools used
- Methodology
- Sample data output
- Benefits and challenges

Refer to `Task1_Report.docx` and `Task2_Report.docx` for full documentation.



## 📌 How to Run

1. Place the XML input file in the same directory as the Python scripts.
2. Run each script using:
   ```bash
   python Task1_Extract_Details.py
   python Task2_Neighbour_cells.py
  
3. Check the generated CSV files in the directory.


