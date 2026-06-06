# QwenChat

QwenChat is a lightweight AI chat application powered by the Qwen Large Language Model running locally through Ollama. The project provides a simple interface for interacting with Qwen models without relying on external cloud APIs, enabling private and offline conversations.

## Features

- Local AI chat using Ollama
- Powered by Qwen language models
- Fast response generation
- Privacy-focused (data remains on your machine)
- Simple and easy-to-use interface
- REST API integration with Ollama
- Lightweight deployment

## Tech Stack

- Python
- Flask
- Ollama
- Qwen Models
- HTML/CSS/JavaScript

## Prerequisites

Before running the project, ensure you have:

- Python 3.10+
- Ollama installed
- A Qwen model pulled locally

Example:

```bash
ollama pull qwen3
````

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/QwenChat.git
cd QwenChat
```

Create a virtual environment:

```bash
python -m venv venv
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Running Ollama

Start the Ollama service:

```bash
ollama serve
```

Verify the model is available:

```bash
ollama list
```

## Running the Application

```bash
python app.py
```

Open your browser and navigate to:

```text
http://localhost:5000
```

## Project Structure

```text
QwenChat/
├── app.py
├── requirements.txt
├── templates/
├── static/
├── README.md
└── screenshots/
```

## How It Works

1. User submits a prompt through the chat interface.
2. Flask receives the request.
3. The application sends the prompt to Ollama.
4. Ollama runs the local Qwen model.
5. The generated response is returned to the user interface.

## Future Improvements

* Conversation history
* Streaming responses
* Multiple model selection
* Dark mode
* User authentication
* Docker deployment

## License

This project is licensed under the MIT License.

## Author

Rushikesh Mohalkar

![User Interface](./images/ui.png)
