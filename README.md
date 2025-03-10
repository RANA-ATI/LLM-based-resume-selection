# Resume Ranking Using Google Cloud, PyDrive, and Gemini AI

## Overview
This project automates the process of ranking resumes based on their relevance to a given job description (JD). It utilizes Google Drive for storage, Google Cloud for computation, PyDrive for authentication, and Gemini AI for natural language processing and ranking. The resumes are extracted from a specified Google Drive folder, processed, and ranked based on a scoring system from 1 to 10, where 1 represents the most relevant resume.

## Features
- Connects to Google Drive and fetches resumes automatically.
- Uses PyDrive for authentication and file access.
- Extracts text from resumes (PDF, DOCX, TXT, etc.).
- Utilizes Gemini AI for natural language processing and ranking.
- Implements prompt engineering techniques for accurate ranking.
- Generates a ranked list of resumes based on JD relevance.
- Provides installation and setup instructions through `requirements.txt`.

## Installation
### Prerequisites
Ensure you have the following installed:
- Python 3.x
- Jupyter Notebook
- Google Cloud SDK
- Google Drive API enabled

### Steps
1. **Clone the Repository**
   ```sh
   git clone https://github.com/your-username/resume-ranking.git
   cd resume-ranking
   ```

2. **Create a Virtual Environment (Optional but Recommended)**
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**
   ```sh
   pip install -r requirements.txt
   ```

4. **Set Up Google Cloud Authentication**
   - Create a Google Cloud project.
   - Enable Google Drive API.
   - Download your `credentials.json` from Google Cloud Console.
   - Place `credentials.json` in the project directory.

## Usage
1. **Run the Jupyter Notebook**
   ```sh
   jupyter notebook
   ```
2. Open the `.ipynb` file in Jupyter Notebook.
3. Follow the steps in the notebook:
   - Authenticate and connect to Google Drive.
   - Fetch resumes from the specified folder.
   - Extract text from resumes.
   - Process the text using Gemini AI.
   - Rank resumes based on relevance to the JD.

## Output
- A ranked list of resumes based on their relevance score (1-10).
- A structured dataset containing resume text, extracted features, and rankings.

## File Structure
```sh
resume-ranking/
│── requirements.txt   # Dependencies
│── credentials.json   # Google Cloud authentication (ignored in .gitignore)
│── resume_ranking.ipynb  # Jupyter Notebook with the main workflow
│── data/              # Folder containing resumes (Google Drive linked)
│── output/            # Ranked results
└── README.md          # Documentation
```

## Contributing
Contributions are welcome! Feel free to fork the repository and submit a pull request.

## License
This project is licensed under the MIT License.

## Author
- [M Wasil Shahzad](https://github.com/RANA-ATI)

