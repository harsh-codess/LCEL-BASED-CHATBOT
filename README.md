# LCEL-based Chatbot with Groq API & LangChain Integration
 
This project is a conversational AI chatbot built using **Groq API**, **LangChain**, and the **Gemma-IT 9B model**. It leverages FastAPI for serving the model and integrating both Groq and LangChain APIs to provide intelligent and responsive interactions. Ideal for exploring and testing AI-driven conversation capabilities.

## Table of Contents



## Features

- **Conversational AI**: Uses **Gemma-IT 9B model** to generate responses to user queries.
- **API Integration**: Groq API and LangChain API are utilized for efficient processing and intelligent responses.
- **Free API Keys**: Built using free API keys for both Groq and LangChain, with potential for upgrades.
- **Seamless OS Function Integration**: Handles API calls using the OS function for easy setup and operation.

---

A chatbot built with powerful AI tools for intelligent conversations.


## Technologies Used

- **Groq API**: High-performance, low-latency inference API for processing requests.
- **LangChain**: A framework for developing language models, enabling the chatbot to handle more complex tasks.
- **9B Gemma-IT Model**: A powerful language model with 9 billion parameters, fine-tuned for chatbots.
- **Python**: Primary programming language used for integration and backend operations.
- **OS Function**: Used to manage system-level operations for API requests and responses.

## Setup and Installation

### 1. Clone the Repository

Start by cloning this repository to your local machine:

```bash
git clone https://github.com/your-username/lcel-chatbot.git
cd lcel-chatbot
```

### 2. Install Dependencies

Install the required Python dependencies. It's recommended to use a virtual environment:

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```
### 3. Set Up API Keys

Make sure to have your **Groq API** and **LangChain API keys**. Create a `.env` file in the root directory of the project, and add your keys like this:

```bash
GROQ_API_KEY=your_groq_api_key
LANGCHAIN_API_KEY=your_langchain_api_key
```
### 4. Run the Chatbot

Once the environment is set up and API keys are configured, run the chatbot script:

```bash
python serve.py
```

### 5. Test the Chatbot

Interact with the chatbot via the FastAPI server or integrate it into any application for real-time responses.

## How to Use

Once the chatbot is running, simply send POST requests to the FastAPI server to interact with the model. You can test it through the FastAPI interface, or use the `client.py` to make requests programmatically.

Example (using `client.py`):

```python
import requests

response = requests.post('http://127.0.0.1:8000/chat', json={'text': 'What is the weather today?'})
print(response.json())
```

## API Keys

This project is configured to work with free API keys from **Groq** and **LangChain**. If you are interested in extending the functionality or increasing the usage limits, consider signing up for paid plans from both providers.

For more information on how to obtain your API keys:

- [Groq API Documentation](https://groq.com/docs/)
- [LangChain API Documentation](https://langchain.com/docs/)

## Project Structure

Here’s an overview of the project’s directory structure:

```
lcel-chatbot/
├── client.py # Client-side script for interacting with the chatbot
├── requirements.txt # List of required Python libraries
├── serve.py # FastAPI app to serve the LangChain model
├── simpllmlCEL.ipynb # Jupyter notebook for experimentation and testing
└── README.md # Project documentation (this file)

```


### Key Files:

- **serve.py**: This file sets up the FastAPI server and integrates LangChain with Groq. The server runs the language model via the API and listens for incoming requests.
- **client.py**: A script that connects to the FastAPI server and interacts with the chatbot through HTTP requests.
- **simpllmlCEL.ipynb**: A Jupyter notebook used for testing the chatbot and refining its behavior before integration into the FastAPI service.


## Contributing

Feel free to fork this repository, create a new branch, and submit a pull request for any improvements or new features. Contributions are welcome!

### Guidelines:

- Write clean, well-commented code.
- Add tests where necessary.
- Follow PEP 8 style guidelines for Python code.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


  


