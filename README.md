# 🎙️ India's Got Latent — AI Stage

An interactive Streamlit web application powered by **LangChain** and **Groq (Llama-3.3-70B)**. Select an act persona—ranging from a comedy roast bot to an Elizabethan playwright—and banter with an AI contestant live on stage with full conversation memory.

---

## 📋 Features

* **Multiple Stage Personas:** Switch seamlessly between unique AI act personas (RoastBot, ShakespeareBot, Emoji Translator, Strict Hostel Warden).
* **Stateful Chat Memory:** Retains conversation history throughout the session using LangChain's `InMemoryChatMessageHistory` and `RunnableWithMessageHistory`.
* **Zero API Prompting:** The Groq API key is pre-configured directly inside the script for immediate execution.
* **Fast Inference:** Powered by Groq's low-latency API running `llama-3.3-70b-versatile`.

---

## 🛠️ Prerequisites

Make sure you have the following installed on your system:

* **Python 3.9** or higher
* **pip** (Python package installer)

---

## 🚀 Setup & Installation

### 1. Download or Clone the Repository

Clone this repository or download the source code files into a local folder:

```bash
git clone [https://github.com/Xebel097/India-s-got-Latent-chatbot.git](https://github.com/Xebel097/India-s-got-Latent-chatbot.git)
cd India-s-got-Latent-chatbot
```
### 2. Set Up a Virtual Environment (Recommended)
Create and activate a virtual environment to manage dependencies:

On macOS / Linux:
```bash
python3 -m venv venv
source venv/bin/activate
```
On Windows:
```DOS
python -m venv venv
venv\Scripts\activate
```
### 3. Install Required Dependencies
Install the necessary Python packages using pip:
```bash
pip install streamlit langchain-groq langchain-core
```
##🔑 API Key Configuration
The code is pre-configured to set your Groq API key directly using os.environ["GROQ_API_KEY"] inside app.py:
```python
import os
os.environ["GROQ_API_KEY"] = "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"
```
##🏃 Running the App
Run the application using Streamlit:

```bash
streamlit run app.py
```
Streamlit will automatically open the app in your default browser at http://localhost:8501.

##📁 Project Structure
Plaintext
├── app.py          # Main Streamlit application
└── README.md       # Project setup and documentation
