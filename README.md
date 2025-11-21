## Conversational AI Chatbot
Project Description
This project implements a sophisticated conversational AI chatbot designed to understand user intent, extract key entities from their queries, and maintain conversation context for more coherent and natural interactions. It serves as a foundational example of building intelligent dialogue systems using modern NLP techniques.




##Features
Intent Recognition: Identifies the user's underlying goal (e.g., 'booking', 'product_inquiry', 'support') to provide relevant responses.
Entity Extraction: Utilizes SpaCy to pinpoint and extract crucial information like dates, products, or specific issues from user inputs.
Conversation Context Management: Remembers previous turns in the conversation to handle follow-up questions and incomplete requests intelligently.
Response Generation: Generates appropriate and contextually relevant responses based on recognized intent and extracted entities.
Performance Evaluation: Includes methods for evaluating chatbot performance using metrics like BLEU and ROUGE scores.
Interactive Command-Line Interface (CLI): A simple interface for real-time interaction with the chatbot.
Technologies and Libraries Used
Python: The core programming language.




##SpaCy: For advanced Natural Language Processing, specifically for entity extraction (en_core_web_sm model).
##NLTK: Used for text tokenization, which is essential for calculating BLEU scores.
##rouge_score: For calculating ROUGE metrics to evaluate response quality.
##random: For selecting random responses from predefined lists.
##transformers (Hugging Face): Although not directly used in the final rule-based/contextual chatbot, it was explored ##for advanced response generation demonstrating its capabilities.
##Setup and Installation
##To set up and run the chatbot, follow these steps:






##Clone the repository (or save the notebook):







# If it were a repository
# git clone <repository_url>
# cd conversational-ai-chatbot
Install dependencies: Ensure you have Python 3.8+ installed. Then, install the required libraries:

##pip install spacy nltk rouge_score
##python -m spacy download en_core_web_sm
##Run the Chatbot CLI: Execute the Python script (or the relevant cells in the notebook) that contains the ##chatbot_response function and the CLI loop.





## Assuming your chatbot code is in a file named chatbot_cli.py
# python chatbot_cli.py
In this notebook, you would run the final code cell that starts the interactive loop.






##How to Interact with the Chatbot
##Once the chatbot CLI is running:






##Type your messages in the prompt and press Enter.
The chatbot will respond based on its understanding of your intent and extracted entities.
To end the conversation, type quit, exit, or bye and press Enter.
Example Interactions:



##Chatbot CLI. Type 'quit', 'exit', or 'bye' to end the conversation.
##You: Hello, I'd like to book an appointment.
##Chatbot: When would you like to book? What date would you prefer?
##You: I want it for next Tuesday.








##Chatbot: When would you like to book? How about next Tuesday?
##You: I'm looking for an iPhone.
##Chatbot: Which product are you interested in?





##You: I need help with my laptop.
##Chatbot: How can I assist you with support? Please describe your issue.
##You: Goodbye.
##Chatbot: Goodbye!
