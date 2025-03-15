# Digital City Assistant

Digital City Assistant is an AI-powered application that provides real-time information about cities through interactive voice commands and data visualizations. Built with modern Python frameworks and APIs, this project enables users to explore various aspects of a city—from attractions and quality metrics to demographics and statistics—using natural language queries.

## Features

- **Voice Interaction:**  
  Use speech recognition and text-to-speech to ask questions and receive spoken answers.

- **City Exploration:**  
  Get detailed information about a chosen city, including points of interest, quality metrics, and statistical data.

- **Data Visualization:**  
  Interactive charts and graphs help visualize city metrics, statistics, and attraction distributions.

- **Real-Time Search:**  
  Leverages DuckDuckGo search integration to fetch up-to-date web information.

- **AI-Powered Responses:**  
  Generates intelligent, context-aware responses using the Groq LLM API via LangChain.

## Demo

*Include a screenshot or GIF demo here to showcase the application in action.*

## Getting Started

### Prerequisites

- **Python 3.7+**  
- **Groq API Key:** A valid key is required to access the Groq LLM service.

### Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/ojalzope/digital-city-assitant.git
   cd digital-city-assitant
   ```

2. **Create a Virtual Environment (Optional but Recommended):**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies:**

   ```bash
   pip install -r requirement.txt
   ```

### Environment Configuration

Create a `.env` file in the root directory (if not already provided) with the following contents:

```
# Replace with your actual Groq API key
GROQ_API_KEY=your_groq_api_key_here

# Debug and application settings
DEBUG=True
DEFAULT_CITY=New York
LOG_LEVEL=INFO
DEBUG_MODE=False

# Voice settings
VOICE_RATE=180
VOICE_VOLUME=0.9
RECOGNIZER_ENERGY_THRESHOLD=300
RECOGNIZER_PAUSE_THRESHOLD=0.8

# Search settings
MAX_SEARCH_RESULTS=5
```

Be sure to replace `your_groq_api_key_here` with your actual Groq API key.

### Running the Application

Launch the application using Streamlit:

```bash
streamlit run digitalcityassistant.py
```

Open the URL provided by Streamlit in your browser to start interacting with the Digital City Assistant.

## Usage

1. **Setup:**  
   In the sidebar, enter your Groq API key and the name of the city you wish to explore, then click **Set City**.

2. **Voice Commands:**  
   - Click **Start Listening** to begin voice input.  
   - Speak your query and then click **Stop Listening** to capture and process your query.
   - Alternatively, use the **Test Microphone** button to verify that your microphone is working correctly.

3. **Text Input:**  
   You can also type your questions directly into the provided text box.

4. **Data Visualizations:**  
   Switch to the **City Visualizations** tab to view interactive charts such as quality metrics, statistical comparisons, and attraction distributions.

5. **About:**  
   The **About** tab offers additional insights into the project's architecture, technologies used, and usage instructions.

## Technologies Used

- **Python** – Core programming language
- **Streamlit** – Web application framework for interactive UI
- **LangChain & Groq LLM API** – Orchestration of language model processing and AI-powered responses
- **SpeechRecognition & gTTS** – Voice recognition and text-to-speech capabilities
- **DuckDuckGo Search** – Real-time search integration for fetching updated information
- **Data Visualization Libraries:**  
  - Pandas, NumPy  
  - Matplotlib, Seaborn, Plotly  
  - Pillow

## Project Structure

```
digital-city-assitant/
├── .env                  # Environment configuration file
├── digitalcityassistant.py  # Main application file
├── requirement.txt       # List of Python dependencies
└── README.md             # This file
```

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes. For major updates, open an issue first to discuss your ideas.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

Developed by [ojalzope](https://github.com/ojalzope).  
Feel free to reach out with questions, suggestions, or feature requests.

---

