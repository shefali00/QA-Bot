PDF Chatbot using Gemini:
	This project implements a chatbot that can answer questions based on the content of uploaded PDF files. It uses Streamlit for the user interface, Google's Generative AI (Gemini) for natural language processing, 	and FAISS for efficient similarity search.
 
Features:
	Upload multiple PDF files
	,Extract text from PDFs
	,Process and chunk text for efficient querying
	,Embed text using Google's Generative AI
	,Perform similarity search on user questions
	,Generate detailed answers using Gemini
https://github.com/shefali00/QA-Bot
Prerequisites:
	Python 3.9 or higher
	Google Cloud account with Generative AI API access

Installation:

	Clone the repository:
		Copygit clone https://github.com/shefali00/QA-Bot
		cd QA-Bot

	Install the required dependencies:
		Copypip install -r requirements.txt

	Set up your Google Cloud credentials:
		Create a .env file in the project root
		Add your Google API key: GOOGLE_API_KEY=your_api_key_here



Usage

	Run the Streamlit app:
	Copystreamlit run app.py

Open your web browser and navigate to http://localhost:8501
Use the sidebar to upload PDF files and process them
Ask questions about the content of the PDFs in the main chat interface

Docker Support:
This project includes a Dockerfile for easy deployment. To build and run the Docker container:

Build the Docker image:
Copydocker build -t pdf-chatbot .

Run the container:
Copydocker run -p 8501:8501 pdf-chatbot
