**MAI 475 - Large Language Model Lab Exercise 1**
This repository contains the implementation of Lab Exercise 1 for the MAI 475 course (Large Language Model) as part of the IV MSAIM program, submitted on 12-06-2024. The lab focuses on building a descriptive question-answering system using a large language model (LLM), exploring prompt engineering, comparing model outputs, and generating sample question-answer pairs.
Project Overview
The lab exercise is implemented in a Google Colab notebook (LLM_QA_System.ipynb) using the Hugging Face Transformers library with the DistilGPT-2 model. The code addresses the following requirements:

Descriptive QA System: Implements a question-answering system that generates detailed responses using natural language generation (NLG).
Prompt Engineering: Demonstrates the impact of different prompt formulations (basic, contextual, guided) on model output, with insights into optimization.
Model Comparison: Compares the response of the implemented model (DistilGPT-2) with simulated outputs from Gemini and ChatGPT for a sample question.
Sample Q&A: Generates three sample question-answer pairs and saves all results to CSV files for submission.

**Features**

Uses DistilGPT-2 for efficient text generation in Google Colab.
Handles padding token issues explicitly for robust model inference.
Saves results (prompt engineering, model comparison, sample Q&A) to CSV files.
Provides insights into prompt engineering and model performance differences.

**Prerequisites**
To run the code, you need:

Google Colab (or a local Python environment with Jupyter support).
Python 3.7+.
Required Python libraries (installed via pip):
transformers
torch
pandas



**Setup Instructions**

Clone the Repository:
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>

**Open in Google Colab:**

Upload LLM_QA_System.ipynb to Google Colab.
Alternatively, download the notebook and run it locally using Jupyter.


Install Dependencies:In the Colab notebook, run the following command in a cell:
!pip install transformers torch pandas


**Run the Notebook:**

Execute all cells in the notebook.
The code will:
Test the QA system with a sample question.
Demonstrate prompt engineering with three prompt variations.
Compare model outputs (DistilGPT-2 vs. simulated Gemini/ChatGPT).
Generate three sample Q&A pairs.
Save results to CSV files (prompt_engineering_results.csv, model_comparison_results.csv, sample_qa_results.csv).




**Download Results:**

After running, download the generated CSV files from Colab for submission.



**Usage**
The notebook is structured to execute all parts of the lab exercise automatically. Key functions include:

qa_system(question, context): Generates a descriptive answer to a given question.
demonstrate_prompt_engineering(): Tests three prompt formulations and analyzes their impact.
compare_models(): Compares DistilGPT-2 output with simulated Gemini/ChatGPT responses.
generate_sample_qa(): Produces three sample question-answer pairs.

**To test a custom question:**

Modify the test_question in the main() function:test_question = "Your custom question here?"


Run the notebook to see the response.

**File Structure**

LLM_QA_System.ipynb: Main Colab notebook containing the implementation.
prompt_engineering_results.csv: Output CSV with prompt engineering results.
model_comparison_results.csv: Output CSV with model comparison results.
sample_qa_results.csv: Output CSV with sample question-answer pairs.
README.md: This file.
**
Notes**

Model Choice: DistilGPT-2 is used for efficiency in Colab. Larger models (e.g., GPT-2, LLaMA) could improve performance but require more resources.
Gemini/ChatGPT Comparison: Responses from Gemini and ChatGPT are simulated due to API access limitations. For accurate comparison, manually input the prompt into their interfaces or use their APIs.
Prompt Engineering Insights: The code demonstrates how prompt structure affects output quality, with detailed insights printed in the notebook.
**
Limitations**

DistilGPT-2 may produce less accurate or shorter responses compared to larger models like ChatGPT or Gemini.
Simulated Gemini/ChatGPT responses are based on typical behavior and may not reflect real outputs.
The code is optimized for Colab; local execution may require additional configuration (e.g., GPU support).

**License**
This project is licensed under the MIT License. See the LICENSE file for details.
Acknowledgments

Hugging Face Transformers library for providing the DistilGPT-2 model.
MAI 475 course instructors for the lab exercise guidelines.

