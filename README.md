# OpenAI Chatbot with Autoprompt
This Python program demonstrates how to interact with OpenAI's GPT-3.5-turbo model using the Chat API, featuring a powerful autoprompt functionality. The autoprompt helps clarify user inputs and ensures that the chatbot provides more accurate and relevant responses. The main goal of this description is to highlight user inputs and their roles in using the program effectively, or at least that's what the AI said.


Tested in:
Python 3.10.10+

OpenAI Python Library: Install it with `pip install openai`



How the program works:


The program works by simulating a conversation between the user and the chatbot. When the user inputs a message, the chatbot processes it and responds accordingly. The autoprompt feature comes into play by taking the user's input, as well as the chatbot's response, and passing them through another instance of the chatbot. This second instance, called the "feedback_chatbot", is instructed to give feedback or help clarify the user's input.


Once the feedback is obtained, it is added to the conversation as if the user themselves provided it. This helps the main chatbot understand the user's intention better and provide more accurate responses. The process repeats continuously, ensuring that the chatbot's responses are consistently improved and fine-tuned based on the user's input and the feedback from the feedback_chatbot.



To interact with the chatbot:


Enter your message and end it with a "`|`" character in a new empty line at the end.

The chatbot will respond with an answer.

If autoprompt is enabled, the program will loop through the autoprompt process, displaying the chatbot's responses.

Remember to set your `api_ key` and customize any settings as needed before running the program. By following these steps, you'll be able to take full advantage of the autoprompt feature to improve the chatbot's responses and better understand user inputs.



How to Use the Program


Clone the repository and navigate to the project folder.

Ensure that the required packages are installed by running `pip install openai`.

Open the main Python file (`gpt-auto-prompter.py`) in a text editor and set the `api_key` variable at the top to your OpenAI API key in str format.

Run the program with `python gpt-auto-prompter.py`.





Key components of the program:


Chatbot: A class that represents a chatbot, with methods for interacting with the OpenAI API and handling the conversation.

Conversation: A class that manages the conversation, keeping track of messages and their roles (user, assistant, or system).

autoprompt: A function that takes the conversation, chatbot, and feedback_chatbot instances and handles the autoprompting process.





User Inputs


The program will prompt users for various inputs to customize their interaction with the chatbot:


`Conversation name`: Provide a name for the conversation. The program will save the conversation history to a JSON file with this name.


   `New or existing conversation`: Choose whether to create a new conversation or load an existing one from a JSON file.


`System message`: Enter a system message, which is a prompt that helps set the context for the conversation with the chatbot.


`Autoprompt`: Choose whether to enable the autoprompt feature by responding with "y" or "n".

   `Autoprompt system message`: If autoprompt is enabled, provide a system message for the autoprompt.

   `Autoprompt message limit`: If autoprompt is enabled, specify the number of messages the autoprompt should use in its feedback loop.
    
    
To stop the program press `CTRL + C` on the `terminal`



When token reaches 4k, program will hault, a feature to forget past mesasges will be implemented at some point



Enjoy interacting with the chatbot and exploring the power of the autoprompt feature!
