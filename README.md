# DataGuard AI — GenAI Data Quality 

DataGuard AI is a GenAI-powered data analysis agent that automatically performs data quality validation on Excel datasets.

The application uses an LLM-powered agent to understand the dataset, dynamically determine relevant validations and analysis, generate Python code, execute the code, review the results, and present the analysis in a user-friendly format.

## 🚀 Features

* Upload Excel files through a Streamlit interface
* Detect and display available Excel sheets
* Select a specific sheet for analysis
* Inspect dataset structure and sample records
* Dynamically identify relevant data quality validations
* Generate Python/Pandas analysis code using an LLM
* Execute generated Python code through a controlled tool
* Automatically review Python execution results
* Handle Python execution errors and retry with corrected code
* Perform exploratory data analysis
* Analyze numerical, categorical, and date columns
* Generate data quality findings and insights

## 🏗️ Architecture

Excel File
↓
Sheet Selection
↓
GenAI Data Analyst Agent
↓
Dataset Inspection
↓
Dynamic Validation & EDA Selection
↓
Python Code Generation
↓
Python Execution Tool
↓
Result Review
↓
User-Friendly Analysis

## 🛠️ Tech Stack

* Python
* Streamlit
* LangChain
* Groq LLM
* Pandas


## ⚙️ How It Works

1. Upload an Excel workbook.
2. The application identifies the available sheets.
3. Select the sheet you want to analyze.
4. The selected sheet is saved as a separate Excel file.
5. The GenAI agent inspects the dataset.
6. The agent dynamically decides which validations and EDA are relevant.
7. The agent generates Python code using Pandas.
8. The generated code is executed through the Python analysis tool.
9. The agent reviews the actual Python output.
10. The final analysis is presented to the user.

## 🔐 Environment Variables

Create a `.env` file locally and add your Groq API key:

```text
GROQ_API_KEY=your_api_key_here
```

Do not upload the `.env` file or expose your API key publicly.

## ▶️ Run Locally

Install the required packages:

```bash
pip install -r requirements.txt
```

Run the Streamlit application:

```bash
streamlit run app.py
```

## 🎯 Project Objective

The goal of DataGuard AI is to demonstrate how GenAI agents can assist data analysts by dynamically understanding datasets, selecting appropriate data quality checks, generating executable analysis code, and converting raw analytical results into meaningful business-facing insights.

