# Research AI Agent

This is a web-based application built using Flask that allows users to generate research papers by leveraging tools such as Wikipedia search and DuckDuckGo search. The application uses Google Generative AI (`gemini-2.0-flash`) for generating research summaries and organizing them into structured Word documents.

---

## 📁 Project Structure

```
.
├── templates
│   ├── index.html        # Home page with input form for research topic
│   ├── results.html      # Results page displaying the research summary
├── .env                  # Environment variables file (for API keys)
├── app.py                # Main Flask application
├── requirements.txt      # Python dependencies
```

---

## 📌 Features

- 🌐 **Web-based Interface:** Accepts research topics via a form.
- 🔍 **Tools Integration:** Uses Wikipedia and DuckDuckGo for fetching information.
- 💬 **Language Model:** Utilizes `gemini-2.0-flash` for generating structured research summaries.
- 📄 **Document Generation:** Generates Word documents with executive summary, sources, and generation date.
- 📥 **Download Feature:** Allows users to download the generated document as a `.docx` file.

---

## 🔧 Installation

1. **Clone the repository:**  
```bash

git clone https://github.com/samyakraka/research-ai-agent.git
cd research-ai-agent
```

2. **Set up a virtual environment (Recommended):**  
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies:**  
```bash
pip install -r requirements.txt
```

4. **Create a `.env` file and add your environment variables:**  
```
API_KEY=your_google_generative_ai_api_key
```

---

## 🚀 Usage

1. **Run the application:**  
```bash
python app.py
```

2. **Open the application in your browser:**  
```
http://127.0.0.1:5000/
```

3. **Enter your research topic and submit.**

4. **View the results and download the generated document.**

---

## 📚 Dependencies

- Flask  
- python-dotenv  
- pydantic  
- langchain  
- langchain_google_genai  
- langchain_core  
- langchain_community  
- docx (python-docx)  
- datetime  

---

## 📁 Example `.env` File

```
API_KEY=your_google_generative_ai_api_key
PORT=5000
```

---

## 📌 Notes

- Ensure that you have valid API keys set up in your `.env` file.
- Customize the `requirements.txt` file if needed by running:  
  ```bash
  pip freeze > requirements.txt
  ```

---

## 📄 License

This project is licensed under the MIT License. Feel free to use and modify it as needed.


