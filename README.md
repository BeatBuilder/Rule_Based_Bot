# Rule_Based_Bot
# RuleBot

This Python code implements a simple chatbot named RuleBot that can converse with a user on a variety of topics. RuleBot is designed to be informative and polite, and it will avoid making claims of sentience or consciousness.

## How it Works

RuleBot is a rule-based chatbot, meaning it relies on a set of predefined rules and responses to interact with the user. The core functionality of RuleBot is encapsulated in the `RuleBot` class. Here's a breakdown of the key methods:

* `__init__()`: Initializes the chatbot with pre-defined negative responses, exit commands, and random starter questions. It also creates a dictionary mapping conversation intents to methods.
* `greet()`: Greets the user, introduces RuleBot, and asks for the user's name. If the user declines to help, the chatbot exits gracefully.
* `make_exit()`: Checks if the user's reply matches any exit commands. If a match is found, the chatbot exits the conversation.
* `chat()`: Starts the conversation loop. The chatbot asks the user a random question and then continues to process the user's replies until an exit command is detected.
* `match_reply()`: Tries to match the user's reply to a conversation intent using regular expressions defined in the `alienbabble` dictionary. If a match is found, the corresponding method is called. Otherwise, the `no_match_intent()` method is called.
* `describe_planet_intent()`, `answer_why_intent()`, `about_intellipaat()`: These methods are triggered based on conversation intents and provide pre-defined responses related to the planet the chatbot is from, its purpose on Earth, and information about Intellipaat.
* `no_match_intent()`: Provides generic responses when the user's input doesn't match any conversation intent.

## Running the Code

1. Save the code as a Python file (e.g., rulebot.py).
2. Open a terminal and navigate to the directory containing the file.
3. Run the code using the following command:

```bash
python rulebot.py
