### **AI-Powered Search Engine Using LangChain and Streamlit**

---

## **1. Introduction**  
The `app.py` file in this repository is a **Streamlit-based AI-powered search engine**, integrating **LangChain** for intelligent search capabilities. This application allows users to query information from sources like **Arxiv, Wikipedia, and DuckDuckGo**, leveraging AI models for real-time responses.

This search engine uses **ChatGroq**, a large language model, alongside LangChain’s **agent-based framework** to enhance search accuracy and efficiency.

---

## **2. Project Description**  
This project aims to create a **user-interactive search assistant** using Python and Streamlit. The application:
✔ Enables users to search for academic papers, general knowledge, and web data.  
✔ Integrates **LangChain agents** with AI models for automated query handling.  
✔ Uses **Streamlit UI** for real-time interactions and structured responses.  

The core idea is to **simulate a conversational AI assistant** that fetches relevant search results and responds dynamically, much like a chatbot with enhanced web search capabilities.

---

## **3. Methodology & Functioning**  

### **Step 1: Importing Libraries and Initializing APIs**  
The application utilizes multiple APIs for retrieving search results:
✔ `ArxivAPIWrapper` – Fetches academic papers from Arxiv.  
✔ `WikipediaAPIWrapper` – Retrieves summaries from Wikipedia.  
✔ `DuckDuckGoSearchRun` – Performs web searches using DuckDuckGo.  

These APIs ensure diverse and **accurate information retrieval**.

### **Step 2: Streamlit-Based UI Setup**  
The `st.title()` method sets up the UI header **"🔎 LangChain - Chat with Search"**, making it visually appealing.

The **sidebar menu** allows users to input their Groq API key, ensuring secure communication with the chatbot.

### **Step 3: Chat Message Initialization**  
The application maintains a **chat history** (`st.session_state["messages"]`), enabling:
✔ Storing previous conversations.  
✔ Allowing AI-generated responses to retain context.  
✔ Creating a chatbot-like **interactive experience**.

### **Step 4: AI Model & LangChain Agent Setup**  
The application initializes `ChatGroq()`, an AI-powered model using the `Llama3-8b-8192` model. This AI model processes user queries efficiently and interacts with search tools.

LangChain’s **AgentType.ZERO_SHOT_REACT_DESCRIPTION** ensures the chatbot **interprets and processes user queries dynamically** without predefined rules.

### **Step 5: Processing User Queries**  
The chatbot receives **user-input queries via `st.chat_input()`** and responds using:
✔ AI-powered **LLM reasoning**.  
✔ Multiple search tools (Arxiv, Wikipedia, DuckDuckGo).  
✔ Streamlit **callback handlers** to display responses.

---

## **4. Potential Challenges**
This project presents several **technical hurdles**, including:

### **1. API Limitations and Rate Restrictions**  
APIs like **Arxiv and Wikipedia** impose request limits. If multiple users access the search engine simultaneously, requests may fail.

### **2. Search Accuracy and Ranking Issues**  
The search engine retrieves multiple results, but ranking **highly relevant answers** remains challenging.

### **3. Performance Optimization**  
Handling multiple search APIs while maintaining **fast response times** requires efficient query processing.

### **4. UI/UX Enhancements**  
The Streamlit UI is functional, but **styling improvements** (better layout, enhanced responsiveness) can enhance user engagement.

### **5. Handling Parsing Errors**  
LangChain agents sometimes struggle with **complex queries**, requiring better error-handling mechanisms.

---

## **5. Running the Streamlit Application**
To **execute the search engine**, follow these steps:

### **Step 1: Clone the Repository**
Run:
```bash
git clone https://github.com/piyush230502/Search_Engine.git
cd Search_Engine
```

### **Step 2: Install Dependencies**
Install required libraries:
```bash
pip install -r requirements.txt
```

### **Step 3: Run the Application**
Execute:
```bash
streamlit run app.py
```

### **Step 4: Enter API Key**
Users must enter a **Groq API key** in the sidebar settings for chatbot functionality.

### **Step 5: Interact with the AI-Powered Search Engine**
The chatbot is now ready to process queries using **LangChain** and multiple search tools.

---

## **6. Requirements for Building the Search Engine**
### **Essential Technologies & Libraries**
✔ **Python (>=3.8)** – Base programming language.  
✔ **Streamlit** – UI framework for interactive chatbot design.  
✔ **LangChain** – AI agent handling for advanced search functionality.  
✔ **ArxivAPIWrapper & WikipediaAPIWrapper** – Specialized search APIs.  
✔ **DuckDuckGo API** – Web search engine integration.  

### **Deployment Requirements**
✔ **Cloud Hosting (Streamlit Cloud, AWS, or Heroku)** – For remote accessibility.  
✔ **Secure API Key Management** – Essential for **Groq API authentication**.  
✔ **Performance Optimization** – To reduce **query processing time**.

---

## **7. Future Improvements**
To further **enhance search capabilities**, developers can implement:
✔ **Search Result Ranking** – Using machine learning techniques for better result ordering.  
✔ **Natural Language Understanding (NLU)** – Improving chatbot reasoning for complex queries.  
✔ **UI Enhancements** – Better themes, dynamic responses, and improved styling.  
✔ **Caching Mechanisms** – Storing recent queries to **reduce API calls and speed up responses**.  

These improvements will make the **AI-powered search engine more efficient, scalable, and user-friendly**.

##**Project Demo Video**
Demo link : https://drive.google.com/file/d/1tjHGEYSXTBsxJDDph9FXCBnhvS_gi-8B/view?usp=sharing
---

## **8. Conclusion**
The `app.py` file represents an **advanced AI-driven search assistant**, leveraging **LangChain’s agent framework and multiple search APIs**. With **Streamlit-based UI**, it offers an intuitive and interactive way for users to perform **real-time searches using AI models**.

With **optimizations in search accuracy, performance, and user experience**, this application can evolve into a **powerful AI-enhanced research assistant**. 🚀  
