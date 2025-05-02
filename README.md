# Resume Analyser NLP

Resume Analyser NLP is a Python-based project that leverages Natural Language Processing (NLP) techniques to analyze resumes, extract key information, and provide meaningful insights. This project is designed to help streamline the resume screening process by identifying important keywords, skills, and other relevant details efficiently.

---

## Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [How It Works](#how-it-works)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

---

## Features
- **Resume Text Processing**: Tokenizes, lemmatizes, and cleans resume text using NLP.
- **Keyword Extraction**: Identifies important keywords and bi-grams from resumes.
- **Stopword Removal and Lemmatization**: Removes unnecessary words and reduces words to their root forms.
- **Customizable Analysis**: Easily adaptable for different industries or resume formats.

---

## Technologies Used
- **Programming Language**: Python
- **Libraries**:
  - `nltk`: Natural Language Toolkit for NLP tasks.
  - `pandas`: Data manipulation and analysis.
  - `numpy`: Numerical computations.
- **Tools**:
  - Jupyter Notebook: For running and developing the project.

---

## Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/KiranYarashi/Resume_Analyser-NLP-.git
   cd Resume_Analyser-NLP-
   ```

2. **Install Dependencies**:
   Ensure you have Python installed (preferably 3.7 or higher). Then, install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. **Download NLTK Resources**:
   Open a Python shell or Jupyter Notebook and run the following commands:
   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('stopwords')
   nltk.download('wordnet')
   ```

4. **Prepare Input File**:
   Place the resumes you want to analyze as plain text files in the project directory. Ensure the file is named `textfile.txt` for the default setup.

---

## Usage

1. **Run the Jupyter Notebook**:
   Open `notebook/main.ipynb` in Jupyter Notebook and execute the cells sequentially.
   ```bash
   jupyter notebook notebook/main.ipynb
   ```

2. **Analyze Resumes**:
   - The notebook will process the text in `textfile.txt`.
   - Extracted keywords and insights will be displayed as outputs in the notebook.

3. **Customize the Analysis**:
   Modify the `nlp()` and `get_key_word()` functions in the notebook to suit your specific requirements.

---

## Project Structure
```
Resume_Analyser-NLP-/
├── notebook/
│   └── main.ipynb          # Main notebook for the project
├── requirements.txt        # Python dependencies
├── textfile.txt            # Sample resume input file
└── README.md               # Project documentation
```

---

## How It Works

1. **Data Preprocessing**:
   - The resume text is loaded from `textfile.txt`.
   - Unnecessary symbols, stopwords, and punctuation are removed.
   - Tokens are lemmatized to their base forms for uniformity.

2. **Keyword Extraction**:
   - The `get_key_word()` function uses `BigramCollocationFinder` from `nltk` to identify frequently occurring word pairs.
   - Results are filtered and returned for analysis.

3. **Output**:
   - Displays a list of extracted keywords and insights, which can be used to evaluate resume content.

---

## Contributing
Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch for your feature or issue.
3. Submit a pull request with a detailed explanation of your changes.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Acknowledgements
- [NLTK](https://www.nltk.org/) for providing powerful NLP tools.
- The open-source community for their contributions and inspiration.
