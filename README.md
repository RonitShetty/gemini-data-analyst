# Gemini Data Analyst

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://your-app-url-here.streamlit.app/)
[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-390/)
[![LangChain](https://img.shields.io/badge/LangChain-Powered-green)](https://langchain.com/)
[![Gemini API](https://img.shields.io/badge/Gemini-1.5%20Flash-orange)](https://deepmind.google/technologies/gemini/)

**Gemini Data Analyst** is an intelligent, conversational analytics dashboard capable of analyzing CSV and Excel files through natural language. 

Built with **Streamlit** and powered by **Google's Gemini 1.5 Flash** model (via LangChain), this application allows users to upload datasets and ask questions like *"Who is the top earner?"* or *"Plot the sales trend over time"* without writing a single line of code or SQL.

---

## 🚀 Key Features

* **🗣️ Natural Language Querying:** Translate plain English questions into Python/Pandas logic automatically.
* **📈 Automated Visualization:** The agent intelligently detects when a chart is needed and generates interactive **Plotly** graphs.
* **🛡️ Secure & Private:** API keys are handled securely. Data is processed in-memory and is wiped after the session ends.
* **📂 Multi-Format Support:** Seamlessly handles both `.csv` and `.xlsx` files.
* **⚡ Reactive UI:** Built with Streamlit for a fast, dark-mode enabled modern interface.

---

## 🛠️ Technical Architecture

The application uses a **Retrieval Augmented Generation (RAG)** adjacent approach where the LLM is provided with the dataframe schema and a Python REPL tool.

* **Frontend:** [Streamlit](https://streamlit.io/) (Web Framework)
* **Orchestration:** [LangChain](https://www.langchain.com/) (Agent Framework)
* **LLM:** [Google Gemini 1.5 Flash](https://ai.google.dev/) (Reasoning Engine)
* **Data Manipulation:** [Pandas](https://pandas.pydata.org/)
* **Visualization:** [Plotly Express](https://plotly.com/python/plotly-express/)

---

## ⚙️ Installation & Local Setup

Follow these steps to run the application on your local machine.

### 1. Clone the Repository
```bash
git clone [https://github.com/your-username/gemini-data-analyst.git](https://github.com/your-username/gemini-data-analyst.git)
cd gemini-data-analyst

```

### 2. Create a Virtual Environment (Optional but Recommended)

```bash
python -m venv venv
# On Windows
venv\Scripts\activate
# On Mac/Linux
source venv/bin/activate

```

### 3. Install Dependencies

```bash
pip install -r requirements.txt

```

### 4. Run the Application

```bash
streamlit run app.py

```

---

## 📖 Usage Guide

1. **Get an API Key:**
* Visit [Google AI Studio](https://aistudio.google.com/) to generate a free Gemini API Key.


2. **Launch the App:**
* Enter your API Key in the sidebar (or set it in `.streamlit/secrets.toml` for persistence).


3. **Upload Data:**
* Drag and drop your CSV or Excel file.


4. **Ask Questions:**
* *Analytical:* "What is the average age of employees in the IT department?"
* *Visual:* "Create a bar chart showing revenue by region."



---

## 📂 Project Structure

```text
gemini-data-analyst/
├── app.py                  # Main application logic (UI + LangChain Agent)
├── requirements.txt        # Python dependencies
├── .gitignore             # Files to exclude from Git
└── README.md               # Project documentation

```

---

## 🔮 Future Roadmap

* [ ] Add support for PDF and text file analysis (RAG).
* [ ] Implement "Download Report" feature to export conversation history.
* [ ] Add support for multiple file uploads simultaneously.
* [ ] Dockerize the application for easier containerized deployment.

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

**Created by [Ronit Shetty](https://github.com/RonitShetty)**


```

```
