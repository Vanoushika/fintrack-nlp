# FinTrack NLP

FinTrack is a financial tracking application that uses Natural Language Processing (NLP) to extract and classify financial data from text inputs.

## 🔧 Features

- Extracts entities like expenses, income, and dates from plain text  
- Categorizes financial data using NLP models  
- Simple and modular Python structure  
- Easily extendable with custom rules or machine learning models  

## 🛠 How to Run

```bash
# 1. Create a virtual environment
python3 -m venv venv
source venv/bin/activate  # On Windows, use venv\Scripts\activate

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run the app
python main.py
```


## 📁 Project Structure
fintrack-nlp/
├── data/                 # Sample text data for testing
├── models/               # Pretrained or custom NLP models
├── utils/                # Utility functions for processing
├── main.py               # Entry point of the application
├── requirements.txt      # Project dependencies
└── README.md             # Project documentation



## 🧠 NLP Capabilities
Named Entity Recognition (NER) to detect key financial terms
Regex-based fallback extraction for unrecognized phrases
Context-aware classification for better categorization

## 🧪 Example Input
"Paid $120 for groceries on June 5th and received salary of $3000 on June 1st."

## Output
[
  {
    "type": "expense",
    "amount": 120,
    "category": "groceries",
    "date": "2024-06-05"
  },
  {
    "type": "income",
    "amount": 3000,
    "category": "salary",
    "date": "2024-06-01"
  }
]


## 🔍 Future Improvements

Integrate with databases for persistent storage
Add web interface or chatbot
Support for multiple languages
Model fine-tuning with financial domain-specific data

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## 📄 License

This project is licensed under the MIT License.

