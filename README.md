
# 🤖 RAG-Based Business QA Bot

This project implements a **Retrieval-Augmented Generation (RAG)** model for answering business-related queries using OpenAI and Pinecone APIs. It uses embedding-based semantic search with a vector database and generates final answers using a GPT model.

---

## 📁 Main File

- `RAG_QA_Bot.ipynb` — Google Colab notebook containing:
  - RAG pipeline setup
  - Document embedding & storage in Pinecone
  - Context retrieval
  - GPT-based answer generation
  - Optional chatbot UI using Gradio

---

## ⚙️ How to Run (Google Colab)

1. Open the notebook in **Google Colab**
2. Install required packages:
   ```bash
   !pip install openai pinecone-client gradio tiktoken
   ```
3. Paste your API credentials (**do not hardcode in public repos**):
   ```python
   openai.api_key = "YOUR_OPENAI_API_KEY"
   pinecone.init(api_key="YOUR_PINECONE_API_KEY", environment="YOUR_PINECONE_ENV")
   ```
4. Modify `business_docs = [...]` to include your own business content.
5. Run all cells and test with a sample question:
   ```python
   print(generate_answer("What services do you offer?"))
   ```

---

## 🔐 Required APIs

- **OpenAI API Key** – Get from [https://platform.openai.com](https://platform.openai.com)
- **Pinecone API Key & Environment** – Get from [https://app.pinecone.io](https://app.pinecone.io)


---

## 📣 Credits

Developed by **Bhanu Prakash**  
Built as part of a QA system project for business knowledge automation.

---

## 🛡️ License

This project is open for academic and research purposes.  
For commercial use or redistribution, please contact the author.
