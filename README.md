# Intelligent-Research-Assistant
Overview
The Intelligent Research Assistant for Professionals is a web-based tool built to assist professionals in answering specific queries by utilizing a combination of machine learning, language models, and document retrieval systems. The assistant processes natural language queries and provides relevant responses sourced from a pre-built vectorstore of documents. It is built using FastAPI for the backend and Streamlit for the frontend, powered by LangChain and OpenAI models.
Key Features:
•	Natural Language Understanding: The assistant can process and understand user queries in natural language.
•	Context-Aware Responses: The assistant retrieves and processes documents related to the query to provide accurate responses.
•	Fast API Integration: FastAPI handles the backend, allowing efficient querying and interaction with the model.
•	Streamlit Interface: The frontend interface allows users to interact with the assistant using a simple web-based form.
Technologies Used:
•	FastAPI: For building the RESTful API backend.
•	Streamlit: For creating the simple web frontend interface.
•	LangChain: For document retrieval and question-answering chain.
•	OpenAI API: For language model-based processing of queries.
•	FAISS: For fast similarity search and document retrieval.
•	dotenv: For securely loading environment variables.
•	Python: The primary programming language.
Usage
1.	Using the Web Interface:
o	Once the Streamlit app is running, open it in a browser.
o	Enter a query in the input field and click "Submit."
o	The system will return a response based on the documents in the vectorstore.
2.	Using the API:
o	You can also interact with the assistant through the FastAPI endpoints.
o	Use a tool like Postman to send a POST request to the /ask endpoint with the following JSON body:
json
Copy code
{
  "query": "What is the capital of France?"
}
o	The response will be in the form:
json
Copy code
{
  "query": "What is the capital of France?",
  "response": "The capital of France is Paris."
}

