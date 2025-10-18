# Akshay's Personal AI Agent

This project is a personal AI agent designed to act as a digital representative for Akshay Karthick on his personal website. The agent is a chatbot built with Gradio and powered by the Gemini API. Its primary purpose is to answer questions related to Akshay's career, background, professional skills, and experience.

## Overview

The AI agent is designed to be a helpful and professional assistant for users visiting Akshay's website. It is strictly programmed to handle inquiries within the scope of Akshay's professional life and will politely decline to answer any off-topic questions. The agent can also record user interest and log questions it cannot answer for future improvements.

## Features

  - **Conversational AI:** A friendly and interactive chatbot interface for users to ask questions.
  - **Personalized Knowledge Base:** The agent's knowledge is based on Akshay's resume and a detailed professional summary.
  - **Tool Integration:** The agent can use tools to:
      - Record a user's email and interest.
      - Log questions that it is unable to answer.
  - **Notifications:** The agent uses Pushover to send real-time notifications when users interact with it.
  - **Strictly Focused:** The agent is designed to only answer questions about Akshay's professional profile and will not engage in general conversation or provide information on other topics.

## How It Works

The application is built in Python and uses the following key technologies:

  - **Gradio:** To create the user-friendly chat interface.
  - **Gemini API:** For the core language model and conversational capabilities. The application uses the `gemini-2.5-flash` model.
  - **Pushover:** For sending push notifications when specific events occur (e.g., a user leaves their contact information).
  - **pypdf:** To read and extract text from Akshay's PDF resume.

The agent's behavior is guided by a detailed system prompt that defines its persona and limitations. The prompt instructs the agent to act as Akshay, answer only professional questions, and use the provided tools when necessary.

## Setup and Installation

To run this project locally, follow these steps:

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/akshaykarthicks/akshay-personal-agents.git
    cd akshay-personal-agents
    ```

2.  **Install system dependencies:**
    The `apt.txt` file lists the required system packages. On a Debian-based system, you can install them using:

    ```bash
    sudo apt-get update && sudo apt-get install -y $(cat apt.txt)
    ```

3.  **Install Python packages:**
    The required Python packages are listed in `requirements.txt`. Install them using pip:

    ```bash
    pip install -r requirements.txt
    ```

4.  **Set up environment variables:**
    Create a `.env` file in the root directory and add the following variables:

    ```
    GOOGLE_API_KEY="YOUR_GOOGLE_API_KEY"
    PUSHOVER_TOKEN="YOUR_PUSHOVER_TOKEN"
    PUSHOVER_USER="YOUR_PUSHOVER_USER_KEY"
    ```

5.  **Add your personal information:**

      - Place your resume in PDF format at `me/Akshaykarthick_s.pdf`.
      - Add your professional summary to `me/summary.txt`.

## Usage

To start the chatbot, run the `app2.py` script:

```bash
python app2.py
env
google_api_key
```

This will launch a local Gradio server. Open the provided URL in your browser to interact with the AI agent.

## Author

**Akshay Karthick S**

  * **GitHub:** [akshaykarthicks](https://github.com/akshaykarthicks)
  * **LinkedIn:** [akshaykarthicks](https://linkedin.com/in/akshaykarthicks)
