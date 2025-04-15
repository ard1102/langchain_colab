# Pet Name Generator 🐾
file: langchain_project1.ipynb
A simple application that generates creative pet names based on type and color, leveraging language models via LangChain.

## Overview

This project demonstrates the integration of language models with a Streamlit interface to create a practical pet name generator. It uses LangChain to handle the prompting and interaction with AI models through OpenRouter, allowing for easy switching between different language models.

## Features

- 🐶 Generate pet names based on animal type and color
- 🎨 Simple, user-friendly interface with Streamlit
- 🔄 Support for multiple AI models (Gemini, DeepSeek)
- 🔌 Easy model switching through OpenRouter integration

## Prerequisites

- Python 3.6+
- Google Colab or similar environment

## Getting Started

### 1. Clone the Repository

Clone this repository to your local machine or open it directly in Google Colab.

### 2. Install Dependencies

The project automatically installs the required dependencies in the first code cell:
```python
pip install langchain openai streamlit python-dotenv langchain_community
```

### 3. Set Up Environment Variables

Create a `.env` file with the following variables:
- `API_KEY`: Your OpenRouter API key
- `DATABASE_URL`: OpenRouter base URL (usually `https://openrouter.ai/api/v1`)

The application includes a utility to help manage this file.

### 4. Run the Application

Execute all code cells in sequence. The last cell starts a Streamlit server and creates a public URL using localtunnel so you can access the web interface.

## How It Works

1. The user selects their pet type and color from dropdown menus
2. Upon clicking "Generate pet name", the application sends a prompt to the selected AI model
3. The model returns creative name suggestions based on the provided information
4. Results are displayed in the Streamlit interface

## Code Structure

- `app.py`: Streamlit frontend interface
- `gen.py`: Core functionality for interacting with language models
- Environment setup cells: For configuration and dependency management

## Note on OpenRouter

This project uses [OpenRouter](https://openrouter.ai/) to access various language models through a unified API. This approach allows for testing different models without changing API endpoints or keys.

Available models in this implementation:
- DeepSeek Chat v3
- Google Gemini Pro
- DeepSeek R1 and R1 Zero

## Future Improvements

- Add more customization options (pet personality, size, etc.)
- Implement result caching to improve performance
- Add image generation for visualizing the named pet
- Expand model selection directly from the interface

---

This is my first project exploring AI agents and LangChain concepts. More projects will be added to this repository as I continue learning and implementing new ideas.
