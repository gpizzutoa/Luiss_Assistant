# README for Python OpenAI Assistant Script

## Overview
This Python script runs a Streamlit Chatbot application that can connect directly with an already created assistant from the openAI Platform

## Requirements
- Python 3.x
- `openai` Python package

## Installation
1. Install the OpenAI Python package:
   ```bash
   pip install openai
   ```

2. Clone or download this script to your local machine.



## Configuration
Create a `constants.py` file with your documentation it should look something like this:
```python
from openai import OpenAI

assistant_id = 'Inster your assistants ID here'  

api_key = "Instert your API Key here"

client = OpenAI(api_key=api_key)
```

## Usage
Run the script using streamlit:
```bash
streamlit run app.py
```

You will be prompted to enter your message. After entering a message, the script will handle the communication with the OpenAI API and display the assistant's response.

## Key Functions
- `submit_message`: Submits a message to the OpenAI API.
- `get_response`: Retrieves messages from a thread.
- `create_thread_and_run`: Creates a new thread and submits the initial user message.
- `pretty_print`: Formats and prints messages for readability.
- `wait_on_run`: Waits for the OpenAI API to process a submitted message.
- `main`: Main function to start the conversational assistant.


## License
MIT

---

*Note: Replace placeholders like `YourUsername` and `PathToScript` with your actual username and script path. Also, ensure you have a valid OpenAI API key.*
