# 🧬 DNA Sequence Analyzer

A full-stack bioinformatics web application designed to analyze DNA sequences, calculate nucleotide composition, identify Open Reading Frames (ORFs), translate DNA into protein sequences, and compare genetic sequences.

The project provides an interactive dashboard for exploring DNA data using React and Flask.

## 🚀 Features

### DNA Sequence Analysis
- Input DNA sequences manually.
- Upload FASTA or TXT files.
- Validate DNA nucleotide characters.
- Calculate total DNA sequence length.
- Count individual nucleotides (A, T, G, C, N).
- Calculate GC content and AT content percentages.

### Sequence Transformation
- Generate complementary DNA sequences.
- Generate reverse complementary DNA sequences.
- Perform DNA-to-RNA transcription.
- Translate DNA sequences into amino acid sequences.

### Genetic Analysis
- Identify Open Reading Frames (ORFs).
- Compare two DNA sequences.
- Calculate sequence identity percentage.
- Detect positional mismatches.
- Calculate sequence length differences.

### Visualization & Reports
- Interactive nucleotide composition chart.
- Display DNA analysis statistics.
- Download analysis results in JSON format.
- Export analysis results in CSV format.
- Store recent analysis history in browser local storage.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| React.js | Frontend development |
| Vite | Development server and build tool |
| JavaScript | Application logic |
| CSS3 | Responsive UI design |
| Flask | Backend API |
| Python | DNA analysis algorithms |
| Recharts | Data visualization |
| Lucide React | Icons |
| Local Storage | Browser-based history |

## 📂 Project Structure

```text
DNA_Sequence_Analyzer/
│
├── frontend/
│   ├── index.html
│   ├── package.json
│   └── src/
│       ├── App.jsx
│       ├── main.jsx
│       └── style.css
│
├── backend/
│   ├── app.py
│   └── requirements.txt
│
└── README.md
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/AMAN-tech-collab/DNA-Sequence-Analyzer.git
```

### 2. Open the Project

```bash
cd DNA-Sequence-Analyzer
```

### 3. Start the Backend

Navigate to the backend folder:

```bash
cd backend
```

Install the required Python packages:

```bash
pip install -r requirements.txt
```

Start the Flask server:

```bash
python app.py
```

The backend will run at:

```text
http://127.0.0.1:5000
```

### 4. Start the Frontend

Open another terminal:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the Vite development server:

```bash
npm run dev
```

Open the localhost URL displayed in the terminal.

## 🔗 API Endpoints

### Health Check

```http
GET /api/health
```

Checks whether the Flask backend is running.

### Analyze DNA Sequence

```http
POST /api/analyze
```

Request:

```json
{
  "sequence": "ATGCGTACGTAGCTAG"
}
```

Returns sequence length, nucleotide counts, GC/AT percentages, complementary sequences, RNA transcript, protein translation, and ORF information.

### Compare DNA Sequences

```http
POST /api/compare
```

Request:

```json
{
  "sequence1": "ATGCGTACGTAG",
  "sequence2": "ATGCGTACGTAA"
}
```

Returns sequence identity, mismatches, and length difference.

## 🧪 Sample DNA Sequence

```text
ATGCGTACGTTAGCTAGCTAGGCCATGAAATAG
```

Paste this sequence into the analyzer to explore the available features.

## 🎯 Project Objective

The primary objective of this project is to develop an interactive bioinformatics tool that simplifies DNA sequence analysis and provides useful insights into nucleotide composition, sequence transformations, genetic comparison, and potential coding regions.

This project demonstrates the practical application of web development, Python programming, and biological sequence analysis.

## 🔮 Future Enhancements

- MongoDB database integration.
- User authentication and profile management.
- Advanced DNA sequence alignment algorithms.
- Machine learning-based DNA classification.
- Mutation visualization and analysis.
- PDF report generation.
- Biological database integration.
- Enhanced ORF detection across all six reading frames.

## ⚠️ Disclaimer

This project is developed for educational and academic purposes.

The included sequence classification uses a simple GC-content-based heuristic. It is not a trained machine learning model and should not be used for clinical diagnosis or medical decisions.

## 👨‍💻 Author

**Aman Kumar**

B.Tech – Computer Science and Technology (CST)

Delhi Technical Campus, Greater Noida

GitHub: [AMAN-tech-collab](https://github.com/AMAN-tech-collab)

---

⭐ If you find this project useful, consider giving it a star!
