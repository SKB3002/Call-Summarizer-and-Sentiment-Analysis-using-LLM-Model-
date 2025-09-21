# 📞 Call Transcript Analyzer

A simple Python + Gradio app that uses the Groq API to analyze customer call transcripts.
It performs summarization and sentiment analysis in real time, and saves results into a CSV file.

## ✨ Features

📝 Input Transcript – Enter or paste any customer call transcript.

⚡ Summarization – Generates a 1–2 sentence summary using Groq’s LLM.

😀 Sentiment Analysis – Detects customer sentiment (Positive, Neutral, Negative).

📂 CSV Export – Automatically saves results into call_analysis.csv with columns:

Transcript | Summary | Sentiment


🎨 Beautiful UI – Built with Gradio and themed for non-technical users.

## 🚀 Tech Stack

Python 3.11+

Gradio
 → for UI

Pandas
 → for CSV handling

Requests
 → for Groq API calls

Groq API
 → LLM for summarization & sentiment

## 🛠️ Installation

Clone this repository:

git clone https://github.com/yourusername/call-transcript-analyzer.git
cd call-transcript-analyzer


Create a virtual environment (recommended):

python -m venv venv
source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows


Install dependencies:

pip install -r requirements.txt


Add your Groq API Key to your environment:

export GROQ_API_KEY="your_api_key_here"     # macOS/Linux
setx GROQ_API_KEY "your_api_key_here"       # Windows

▶️ Usage

Run the app with:

python app.py


Gradio will open a local URL in your browser:

http://127.0.0.1:7860

## 📂 Example
Input Transcript:
Hi, I tried booking a slot yesterday but the payment failed. 
I need this sorted quickly as I don’t want to lose my spot.

Output:

Summary: Customer faced a payment failure while booking a slot.

Sentiment: Negative

✅ Saved automatically into call_analysis.csv

