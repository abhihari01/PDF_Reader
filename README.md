# PDF_Reader
Requirements:
•	Langchain
•	OpenAI
•	Streamlit
•	PyPDF2
•	Python-dotenv
•	Tiktoken
•	Faiss-cpu

To install above requirements, run below code in terminal:
pip install langchain openai streamlit PyPDF2 python-dotenv tiktoken faiss-cpu 

Enter your api key in “.env” file

Enter below code in terminal to run the app:
streamlit run app.py

After running the above code, you can use website in below URL:
http://localhost:8501/

Working of the application:
The application reads the PDF and splits the text into smaller chunks that can be then fed into a LLM. It uses OpenAI embeddings to create vector representations of the chunks. The application then finds the chunks that are semantically similar to the question that the user asked and feeds those chunks to the LLM to generate a response.
