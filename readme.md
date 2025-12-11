# Langgraph Chartbot

## Overview

Langgraph Chartbot is an AI-powered chatbot application built using Langchain, Streamlit, and OpenAI. It leverages the Langgraph library to create a state graph for managing chatbot states and interactions. The project includes multiple frontend implementations and a backend for handling chatbot logic.

## Features

-   **Backend**: Implements a chatbot using Langgraph and OpenAI's ChatGPT.
-   **Frontend**: Provides three Streamlit-based user interfaces:
    -   `streamlit_frontend.py`: Basic chatbot interface.
    -   `streamlit_frontend_streaming.py`: Streaming responses in the chatbot.
    -   `streaming_frontend_threading.py`: Threaded streaming responses.
-   **State Management**: Uses Langgraph's `StateGraph` for managing chatbot states.
-   **Checkpointing**: In-memory checkpointing for saving chatbot states.

## Installation

1. Clone the repository:

    ```bash
    git clone <repository-url>
    cd Langgraph_chartbot
    ```

2. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

3. Set up environment variables:
    - Create a `.env` file in the root directory.
    - Add your OpenAI API key:
        ```env
        OPENAI_API_KEY=your_openai_api_key
        ```

## Usage

### Backend

The backend is implemented in `langgraph_backend.py`. It defines the chatbot logic and state graph. You can use it as a standalone module or integrate it with the provided frontends.

### Frontend

#### Basic Chatbot Interface

Run the basic chatbot interface:

```bash
streamlit run streamlit_frontend.py
```

#### Streaming Responses

Run the streaming chatbot interface:

```bash
streamlit run streamlit_frontend_streaming.py
```

#### Threaded Streaming Responses

Run the threaded streaming chatbot interface:

```bash
streamlit run streaming_frontend_threading.py
```

## File Structure

-   `langgraph_backend.py`: Backend logic for the chatbot.
-   `streamlit_frontend.py`: Basic Streamlit frontend.
-   `streamlit_frontend_streaming.py`: Streamlit frontend with streaming responses.
-   `streaming_frontend_threading.py`: Streamlit frontend with threaded streaming responses.
-   `requirements.txt`: List of dependencies.
-   `readme.md`: Project documentation.

## Dependencies

The project uses the following libraries:

-   `Langchain`
-   `langgraph`
-   `Langchain-Core`
-   `OpenAI`
-   `Langchain-OpenAI`
-   `Langchain-Experimental`
-   `Langchain-Community`
-   `Langchain-Anthropic`
-   `Langchain-Google-GenAI`
-   `Google-GenerativeAI`
-   `Streamlit`

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

## License

This project is licensed under the MIT License.
