# OpenAI Chatbot with Autoprompt
This Python program demonstrates how to interact with OpenAI's GPT-3.5-turbo model using the Chat API, featuring a powerful autoprompt functionality. The autoprompt helps clarify user inputs and ensures that the chatbot provides more accurate and relevant responses. The main goal of this description is to highlight user inputs and their roles in using the program effectively, or at least that's what the AI said.

Tested in:
Python 3.10.10+

OpenAI Python Library: Install it with `pip install openai`

Autoprompt and Interacting with the Chatbot
The main feature of this program is the autoprompt, which helps users get more accurate and relevant responses from the chatbot by clarifying their inputs, or wild outputs, this is completely untested.


To interact with the chatbot:

Enter your message and end it with a "`|`" character in a new empty line at the end.

The chatbot will respond with an answer.

If autoprompt is enabled, the program will loop through the autoprompt process, displaying the chatbot's responses.

At any point, users can choose to update or not update the conversation file by responding to the "don't update file?" prompt with "y" or "n".


How to Use the Program

Clone the repository and navigate to the project folder.

Ensure that the required packages are installed by running `pip install openai`.

Open the main Python file (`gpt-auto-prompter.py`) in a text editor and set the `api_key` variable at the top to your OpenAI API key in str format.

Run the program with `python gpt-auto-prompter.py`.



User Inputs

The program will prompt users for various inputs to customize their interaction with the chatbot:


`Conversation name`: Provide a name for the conversation. The program will save the conversation history to a JSON file with this name.


   `New or existing conversation`: Choose whether to create a new conversation or load an existing one from a JSON file.


`System message`: Enter a system message, which is a prompt that helps set the context for the conversation with the chatbot.


`Autoprompt`: Choose whether to enable the autoprompt feature by responding with "y" or "n".

   `Autoprompt system message`: If autoprompt is enabled, provide a system message for the autoprompt.

   `Autoprompt message limit`: If autoprompt is enabled, specify the number of messages the autoprompt should use in its feedback loop.
    
    
To stop the program press `CTRL + C` on the `terminal`

Enjoy interacting with the chatbot and exploring the power of the autoprompt feature!
