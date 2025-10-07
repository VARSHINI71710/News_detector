📰 Fake News Detector using BERT

This project is an AI-based Fake News Detection System built using the BERT (Bidirectional Encoder Representations from Transformers) model.
It classifies news as Real or Fake based on its content.

🚀 Features

Uses BERT transformer model for text classification

Gradio Web Interface for user input and live prediction

Detects fake news based on semantic understanding

Easily deployable and extendable

🧠 Model Information

The project uses a fine-tuned BERT model stored as model.safetensors.

⚠️ The trained model file (model.safetensors, ~255 MB) is not included in this repository because of GitHub’s 100 MB file limit.

You can download the model from this link and place it inside the bert_fake_news_model folder:

🔗 Download Model (Google Drive / Hugging Face link here)

🧩 Project Structure
📂 Fake-News-Detector/
 ┣ 📂 bert_fake_news_model/
 ┃ ┣ config.json
 ┃ ┣ model.safetensors     ← (download and place here)
 ┃ ┣ vocab.txt
 ┃ ┣ tokenizer.json
 ┃ ┗ tokenizer_config.json
 ┣ app.py
 ┣ requirements.txt
 ┗ README.md

🛠️ Installation

Clone the repository

git clone https://github.com/VARSHINI71710/News_detector.git
cd News_detector


Create a virtual environment (optional but recommended)

python -m venv venv
venv\Scripts\activate   # (Windows)


Install dependencies

pip install -r requirements.txt


Download the model file and place it inside:

bert_fake_news_model/model.safetensors

💻 Run the App
python app.py


Then open the Gradio interface in your browser — you can enter a news headline or paragraph to test it.

🧾 Example

Input:

"Government launches new digital initiative for farmers."

Output:

✅ Real News

Input:

"Aliens have landed and taken over the internet!"

Output:

❌ Fake News

⚙️ Technologies Used

Python 🐍

Transformers (Hugging Face) 🤗

PyTorch

Gradio

Pandas & NumPy# News_detector
