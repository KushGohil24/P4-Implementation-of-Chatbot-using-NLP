# Recipe Chatbot using NLP

## Overview
This project implements a recipe chatbot using Natural Language Processing (NLP) techniques. The chatbot is designed to assist users with recipe suggestions, quick meals, healthy dishes, Indian street food, and more. It identifies user intents and provides accurate and relevant responses based on predefined patterns and responses. The project leverages `nltk` for natural language processing, `scikit-learn` for machine learning, and `streamlit` for building an interactive web interface.

---

## Features
- Understands user intents such as greetings, recipe queries, and farewells.
- Offers a variety of recipe suggestions, including:
  - Popular recipes
  - Indian dishes
  - Healthy meals
  - Quick-to-make recipes
  - Indian street food
- Built using Python with modular and extensible code for easy customization.
- Simple and user-friendly web interface.

---

## Technologies Used
- **Python**
- **NLTK**
- **Scikit-learn**
- **Streamlit**
- **JSON** for storing intents data

---

## Installation

### 1. Clone the Repository
```bash
git clone <repository-url>
cd <repository-directory>
```

### 2. Create a Virtual Environment (Optional but Recommended)
```bash
python3 -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

### 3. Install Required Packages
```bash
pip install -r requirements.txt
```

### 4. Download NLTK Data
```python
import nltk
nltk.download('punkt')
```

---

## Usage
To run the chatbot application, execute the following command:
```bash
streamlit run app.py
```

Once the application is running, you can interact with the chatbot through the web interface. Type your query in the input box and press Enter to get recipe suggestions or responses.

---

## Intents Data
The chatbot’s behavior is defined by the `intents.json` file. It includes tags, patterns, and responses to manage conversation flows. You can modify this file to add new recipes or customize the chatbot’s responses. 

Example of a tag for recipe suggestions:
```json
{
    "tag": "quick_recipes",
    "patterns": [
        "I need a quick recipe",
        "Can you suggest a fast meal?",
        "Give me something quick to make"
    ],
    "responses": [
        "Try a grilled cheese sandwich or a quick stir-fry!",
        "How about a 5-minute mug cake?"
    ]
}
```

---

## Conversation History
The chatbot saves the conversation history in a CSV file (`chat_log.csv`). You can view past interactions for analysis or debugging purposes.

---

## Contributing
Contributions to this project are welcome! If you have suggestions for improvements, additional recipes, or new features, feel free to open an issue or submit a pull request.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments
- **NLTK** for natural language processing.
- **Scikit-learn** for implementing machine learning techniques.
- **Streamlit** for building the interactive web interface.

---

Replace `<repository-url>` and `<repository-directory>` with your actual repository URL and project directory name. Modify sections to align closely with your project details.
