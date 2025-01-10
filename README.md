# **Session-Based Conversational AI with RAG**

## **Project Overview**
This project demonstrates a conversational AI system using Retrieval-Augmented Generation (RAG). The system integrates session-based chat history, document embedding, vector search, and a robust question-answering mechanism based on PDFs, websites, and other documents.

---

## **Step-by-Step Setup Guide**

### **1. Install Python 3.11.5**
Ensure Python 3.11.5 is installed on your system. You can download it from the [official Python website](https://www.python.org/downloads/release/python-3115/).

Check the installation:
```bash
python3 --version
```
Ensure it shows `Python 3.11.5`.

---

### **2. Create a Project Directory**
1. Create a folder for your project:
```bash
mkdir conversational_ai_project
cd conversational_ai_project
```

---

### **3. Create a Virtual Environment**
1. Set up a virtual environment inside the project folder:
```bash
python3 -m venv venv
```
2. Activate the virtual environment:
   - On Linux/Mac:
     ```bash
     source venv/bin/activate
     ```
   - On Windows:
     ```bash
     venv\Scripts\activate
     ```

---

### **4. Create `requirements.txt` File**
1. In the project directory, create a file named `requirements.txt` with the following content:
```plaintext
langchain
torch
chromadb
sentence-transformers
bs4
dotenv
```

2. Install the dependencies:
```bash
pip install -r requirements.txt
```

---

### **5. Create a `.env` File**
1. In the project directory, create a file named `.env`.
2. Add the following content:
```plaintext
GROQ_API_KEY=your_groq_api_key
HF_TOKEN=your_huggingface_token
```
3. Replace `your_groq_api_key` and `your_huggingface_token` with the actual keys (instructions below).

---

### **6. Generate API Keys and Tokens**

#### **6.1 GROQ API Key**
1. Go to the [GROQ API Dashboard](https://groq.com/).
2. Sign up or log in to your account.
3. Navigate to the API Keys section and create a new key.
4. Copy the key and paste it into the `.env` file under `GROQ_API_KEY`.

#### **6.2 Hugging Face Token**
1. Visit the [Hugging Face Website](https://huggingface.co/).
2. Sign up or log in to your account.
3. Go to your profile, then navigate to **Settings** > **Access Tokens**.
4. Create a new token with the required permissions.
5. Copy the token and paste it into the `.env` file under `HF_TOKEN`.

---

### **7. Use the Provided Notebooks**
This project provides two Jupyter Notebook files for different use cases:

1. **`chatbot_with_website_integration.ipynb`**: For question-answering based on website content.
2. **`pdf_chatbot.ipynb`**: For question-answering based on PDF documents.

#### **Steps to Run a Notebook**
1. Ensure your virtual environment is active:
   ```bash
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
2. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
3. Open the desired notebook (`chatbot_with_website_integration.ipynb` or `pdf_chatbot.ipynb`).
4. Follow the instructions inside the notebook to load documents and query the chatbot.

---

### **8. Run the Application (Optional)**
If you prefer not to use the notebooks, you can convert them into Python scripts or create a custom `main.py` file to orchestrate the chatbot.

---

## **Usage Tips**
- Ensure your documents (PDFs, websites) are properly loaded in the respective notebooks.
- Use unique session IDs to maintain chat continuity.
- Test with different document types to validate the system's robustness.

---

## **Support**
If you encounter issues or need further assistance, feel free to raise an issue in the repository or contact the project maintainer.

---

## **Connect With Me**
For any queries or collaboration opportunities, feel free to connect with me on [LinkedIn]([https://www.linkedin.com/in/h-m-nahid-kawsar/](https://www.linkedin.com/in/h-m-nahid-kawsar-232a86266/).

