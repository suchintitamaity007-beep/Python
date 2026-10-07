def get_chatbot_reply(user_input):
    """Function to determine the chatbot"s response based on rules."""
    user_input=user_input.lower().strip()

    if user_input=="hello":
        return "Hi!"
    elif user_input=="how are you":
        return "I'm fine, thanks!"
    elif user_input=="bye":
        return "Bye!"
    elif user_input=="My name is Suchintita":
        return "Hey, Suchintita!"
    elif user_input=="i need your help":
        return "I am here to help you!"
    else:
        return "I don't understand, could you rephrase that?"

def start_chatbot():
    """Main loop to handle user input and output"""
    print("Chatbot: Hello! Type something to start chatting (type 'bye' to stop)")

    while True:
        user_input=input("You: ")

        reply=get_chatbot_reply(user_input)

        print(f"Chatbot: {reply}")

        if user_input.lower().strip=="bye":
            break
start_chatbot()
# Python
Created a chatbot using python
