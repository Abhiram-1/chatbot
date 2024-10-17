# Claude Chatbot with AWS Bedrock and Streamlit

## Overview

This project implements an interactive chatbot using AWS Bedrock's Claude model, integrated with LangChain for conversation management and Streamlit for the user interface. The chatbot is designed to engage in friendly conversations, provide detailed responses, and maintain context throughout the interaction.

## Features

- Integration with AWS Bedrock using the Claude v2 model
- Conversational memory to maintain context
- User-friendly interface built with Streamlit
- Easy-to-use chat input for seamless interaction
- Configurable AWS settings for customization

## Prerequisites

Before you begin, ensure you have the following:

- Python 3.7 or higher
- An AWS account with access to Bedrock
- AWS credentials (Access Key ID and Secret Access Key)

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/your-username/claude-chatbot.git
   cd claude-chatbot
   ```

2. Create a virtual environment (optional but recommended):
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

## Configuration

1. Create a `.env` file in the project root directory.
2. Add your AWS credentials to the `.env` file:
   ```
   AWS_ACCESS_KEY_ID=your_access_key_id
   AWS_SECRET_ACCESS_KEY=your_secret_access_key
   AWS_DEFAULT_REGION=us-east-1
   ```

## Usage

To run the chatbot:

1. Ensure you're in the project directory and your virtual environment is activated (if used).
2. Run the Streamlit app:
   ```
   streamlit run app.py
   ```
3. Open your web browser and navigate to the URL provided by Streamlit (usually `http://localhost:8501`).
4. Start chatting with the bot by typing your messages in the input box at the bottom of the interface.

## Project Structure

```
chatbot_project/
├── app.py                  # Main Streamlit application
├── requirements.txt        # Project dependencies
├── config/
│   └── aws_config.py       # AWS configuration file
├── .env                    # Environment variables (not in version control)
└── README.md               # Project documentation
```

## Customization

You can customize the chatbot's behavior by modifying the following:

- `app.py`: Adjust the conversation prompt or model parameters.
- `config/aws_config.py`: Change AWS configuration settings.

## Troubleshooting

If you encounter any issues:

1. Ensure all dependencies are correctly installed.
2. Verify that your AWS credentials are correct and have the necessary permissions.
3. Check that you're using a compatible Python version.

