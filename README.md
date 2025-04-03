# AUTOGRADER
# AI-Powered Answer Grading System

## Overview

This project is an AI-powered grading assistant designed to **automate the grading of student answer sheets** based on a provided question paper. It extracts questions, evaluates answers, and provides feedback using **Google's Gemini API**.

## Features

- **Upload Question Papers & Answer Sheets** in Markdown format
- **AI-driven Grading** based on grading scheme in the question paper
- **Automatic Keyword Detection** (AI figures out relevant keywords)
- **Handles Random Order of Answers** and maps them correctly
- **Considers Internal Choice Questions**
- **Strictness Level Control (1-5)** to adjust grading leniency
- **Final Score Calculation & Improvement Suggestions**

## Project Structure

```
📦 AI-Answer-Grading
├── main.ipynb               # Jupyter Notebook containing the full project
├── requirements.txt         # Python dependencies
├── README.md                # Documentation
```

## Setup Instructions

### Install Dependencies

```sh
pip install google-generativeai google-colab
```

### Set Up API Key

Before running the project, set up your **Google Gemini API key**:

```python
import google.generativeai as genai
import getpass
api_key = getpass.getpass("Enter your Gemini API Key: ")
genai.configure(api_key=api_key)
```

### Run the Grading System

Open and run **main.ipynb** in Jupyter Notebook.

## Usage

1. **Upload the Question Paper** (Markdown format) once.
2. **Upload Answer Sheets** multiple times for different students.
3. The AI extracts text, maps answers, evaluates responses, and provides **detailed feedback with scoring**.
4. Adjust **strictness level (1-5)** for more or less leniency in grading.
5. Get a **final score and improvement summary** for each student.

## How It Works

- The AI **parses** the question paper to identify grading criteria.
- It **matches** student answers to the correct questions, even if unordered.
- It **evaluates** based on **keywords, completeness, and logical correctness**.
- Finally, it **assigns scores** and suggests areas for improvement.

## Future Improvements

- Add **support for diagram-based answers**
- Generate **detailed analytics & performance trends**
- Implement **multi-language support** for grading

## License

This project is **open-source** under the MIT License.

## Contribute

Pull requests & suggestions are welcome! If you find this project helpful, **leave a star on GitHub**!

---

**Let's make AI-driven education accessible to all!**


