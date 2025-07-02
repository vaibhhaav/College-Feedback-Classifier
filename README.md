# College-Feedback-Classifier
📊 College Feedback Classifier
This project uses a large language model (LLM) to classify college feedback into different categories (e.g., Positive, Negative, Neutral). The goal is to analyze qualitative student feedback and assist academic institutions in deriving actionable insights.

🚀 Features
Utilizes Hugging Face transformers for natural language processing

Uses mistralai/Mistral-7B-Instruct-v0.2 model for instruction-based classification

Categorizes textual feedback into clear sentiments or themes

User-friendly prompt design for zero-shot classification

Easily customizable for other text classification tasks

🧠 Model Used
Model: mistralai/Mistral-7B-Instruct-v0.2

Provider: Hugging Face 🤗

API Access: Hugging Face transformers with AutoModelForCausalLM and AutoTokenizer

📦 Requirements
Install dependencies using:

bash
Copy
Edit
pip install transformers accelerate
📁 Project Structure
bash
Copy
Edit
.
├── College_Feedback_Classifier.ipynb  # Main notebook
├── README.md                                   # Project documentation
📝 How It Works
Load Pretrained Model and Tokenizer
Initializes the Mistral model and tokenizer using transformers.

Design Prompt Template
Prompts are structured to guide the model in classifying feedback correctly:

css
Copy
Edit
<s>[INST] Classify the following feedback: "{feedback}" [/INST]
Generate Model Output
The feedback text is passed through the model, and it returns the predicted category.

Result Extraction
The output is parsed and cleaned for readability.

📌 Sample Prompt
python
Copy
Edit
feedback = "The faculty members are very helpful, but the mess food needs improvement."
prompt = f"<s>[INST] Classify the following feedback: \"{feedback}\" [/INST]"
🔧 Customization
You can customize the classification categories by modifying the prompt or fine-tuning the model further.

📈 Future Work
Add support for multilingual feedback

Deploy as a web app using Streamlit or Flask

Include explainability (why a particular feedback was classified a certain way)

🤝 Contributing
Pull requests and feedback are welcome. If you’d like to contribute, fork the repo and submit a PR.

📜 License
This project is for educational and research purposes only.
