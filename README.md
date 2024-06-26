# LLM Quiz Wizard - LLM-Powered Quiz Generator
[CLICK HERE TO TRY IT ONLINE](https://llm-quiz-wizard.streamlit.app/) <br> <br>
![ezgif-2-9b593fe36d](https://github.com/AvivGelfand/LLM-Quiz-App/assets/63909805/c12508a5-a7c1-4f99-a384-a03aa44e1cc3)


LLM Quiz Wizard is a web application that generates quiz questions using a large language model (LLM). This app leverages advanced natural language processing capabilities to create engaging and challenging quizzes on various topics.

## Features

- Generate quiz questions dynamically using the LLM [LLaMA3](https://huggingface.co/meta-llama/Meta-Llama-3-70B-Instruct) 70b.
- The language models are called in a lightning-fast LPU engine of [Groq](https://groq.com/).
- Supports various topics and difficulty levels.
- User-friendly interface with [Streamlit](https://streamlit.io/).
- Easily extensible for additional features and customization.

## Installation

To get started, clone the repository and install the required dependencies:

```bash
git clone https://github.com/AvivGelfand/LLM-Quiz-App.git
cd LLM-Quiz-App
pip install -r requirements.txt
```

## Usage

To use Groq's API in your Streamlit application, you need to obtain an API key from Groq and configure your Streamlit app to use it. First, sign up for an account at [Groq's website](https://groq.com) and navigate to the API section in your account settings to generate a new API key. Copy the generated key. Next, locate the `streamlit.toml` file in your Streamlit app's root directory. If it doesn't exist, create a new file named `streamlit.toml`. Add the following lines to the file:

```toml
[general]
GROQ_API_KEY = "your_api_key_here"
```

Replace `"your_api_key_here"` with the key you copied earlier. Save the `streamlit.toml` file. Your Streamlit application is now configured to use the Groq API key for authentication, allowing seamless integration with Groq's services.

Run the application with Streamlit:

```bash
streamlit run app.py
```

## File Structure

- `app.py`: Main application file for Streamlit.
- `llm_operator.py`: Handles interactions with the language model.
- `prompts.py`: Contains the prompts and prompt customizing functions used to generate quiz questions.
- `requirements.txt`: Lists the required Python packages.
- `README.md`: Project documentation.
- `.gitignore`: Specifies files that are to be ignored in version control.



