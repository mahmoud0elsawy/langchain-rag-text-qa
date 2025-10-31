# 🧠 LangChain RAG Text QA

A simple project demonstrating how to use **RAG (Retrieval-Augmented Generation)**  
to answer questions based on the content of a text file using **LangChain** and **OpenAI API**.

---

## 📂 Project Structure

```
langchain-rag-text-qa/
│
├── data.txt              # The source text file
├── main.py               # Main script that loads data, creates the index, and answers questions
├── requirements.txt      # Required dependencies
└── README.md             # Project documentation
```

---

## ⚙️ How It Works

This project combines **Retrieval** and **Generation** to create a simple intelligent Q&A system.

1. Loads the text file `data.txt`.
2. Converts the text into **embeddings** using OpenAI’s embedding model.
3. Creates a **vector index** using LangChain.
4. When you ask a question, it retrieves the most relevant part of the text.
5. Sends that part to an OpenAI model to generate an accurate, context-based answer.

---

## 🧰 Requirements

Install the required dependencies:

```bash
pip install openai langchain langchain_community langchain_openai
```

---

## 🔑 Setting Up OpenAI API Key

Before running the project, you need to set your OpenAI API key as an environment variable.

### 🪟 On Windows:
```bash
setx OPENAI_API_KEY "your_api_key_here"
```

### 🐧 On Linux / macOS:
```bash
export OPENAI_API_KEY="your_api_key_here"
```

---

## 🚀 Running the Project

After placing your text inside `data.txt`, run the script with your question as an argument:

```bash
python main.py "Your question here"
```

### Example:
```bash
python main.py "What does the file contain?"
```

---

## 💡 Example Output

```
Question: What does the file contain?
Answer: The file contains information about how to implement RAG using LangChain and OpenAI.
```

---

## 🧠 Technologies Used

- **Python**
- **LangChain**
- **OpenAI API**
- **text-embedding-ada-002** for embeddings
- **RAG (Retrieval-Augmented Generation)** architecture

---

## 🎯 Project Idea

This project serves as a simple example of modern **AI systems** that combine  
**information retrieval** and **language generation** — similar to the architecture  
used in advanced chatbots and intelligent document assistants.

---

## 👨‍💻 Author

**Mahmoud Magdy**  
📧 mahmoud0magdy4@gmail.com  
📍 Egypt  

---

## 📜 License

This project is open-source and intended for educational purposes.  
You are free to use and modify it with proper attribution.
