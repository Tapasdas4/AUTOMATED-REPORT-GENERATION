*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: TAPAS RANJAN DAS

*INTERN ID*:CT08OQJ

*DOMAIN*: PYTHON PROGRAMMING

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTHOSH KUMAR

import nltk
import random
from nltk.chat.util import Chat, reflections

# Download necessary NLTK resources
nltk.download('punkt')

# Define patterns and responses for the chatbot
pairs = [
 (r"hi|hello|hey", ["Hello!", "Hi there!", "Hey! How can I help you?"]),
 (r"what is your name?", ["I am a chatbot, created to assist you.", "I'm a friendly chatbot!"]),
 (r"how are you?", ["I'm doing great, thank you!", "I'm just a bot, but I'm doing well!"]),
 (r"(.*) your favorite color?", ["I don't have a favorite color, but I think blue is nice!"]),
 (r"what is (.*)?", ["I'm sorry, I don't have information about %1.", "Hmm, I don’t know about %1. Could you clarify?"]),
 (r"(.*) help (.*)", ["Sure! How can I assist you?", "What do you need help with?"]),
 (r"(.*)", ["Sorry, I didn’t quite understand that. Could you rephrase?", "I'm not sure how to respond to that. Could you ask something else?"]),
]

# Create a chatbot using the pattern-response pairs
chatbot = Chat(pairs, reflections)

# Function to start the chatbot conversation
def chat():
 print("Hello! I am your chatbot. Type 'quit' to end the chat.")
 while True:
 user_input = input("You: ")
 if user_input.lower() == 'quit':
 print("Chatbot: Goodbye!")
 break
 response = chatbot.respond(user_input)
 print(f"Chatbot: {response}")

# Start the chatbot
if __name__ == "__main__":
 chat()

View Tapas ranjan’s profileTapas ranjan Das
Tapas ranjan Das  8:08 PM
Click or press enter to display in the image preview
Samaresh Das sent the following messages at 8:22 PM
View Samaresh’s profileSamaresh Das
Samaresh Das (He/Him)  8:22 PM
## Description
This Python project reads data from a CSV file, analyzes it, and generates a PDF report using **FPDF**. The script specifically calculates the average game length from the CSV dataset.

## Features
✅ Reads and processes a CSV file.
✅ Extracts numerical data (game lengths) for analysis.
✅ Computes the average game length using **NumPy**.
✅ Generates a formatted PDF report using **FPDF**.

## Requirements
- Python 3.x
- `numpy` (for numerical analysis)
- `fpdf` (for generating PDF reports)

## Installation & Usage

### 1. Clone the Repository

### 2. Install Dependencies

pip install numpy fpdf

### 3. Run the Script

python analysis_script.py

## Input
- A CSV file containing game data, where the second column represents game lengths.
- Example:
- Game,Game Length
Game 1,30.5
Game 2,35.2
Game 3,36.0
Game 4,33.8


## Output
- A PDF report (`analysis_report.pdf`) containing the average game length.

## Example Output

Report generated: analysis_report.pdf

![Image](https://github.com/user-attachments/assets/ca82da3f-ec33-433a-8a44-cec9d2229b6b)

