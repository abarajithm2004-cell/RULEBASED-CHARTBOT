# Simple Rule-Based Chatbot

def chatbot():
    print("🤖 ChatBot: Hello! I am a simple chatbot. Type 'bye' to exit.")
    while True:
        user_input = input("You: ").lower()  # convert to lowercase for easy matching

        if "hello" in user_input or "hi" in user_input:
            print("🤖 ChatBot: Hi there! How can I help you today?")
        elif "how are you" in user_input:
            print("🤖 ChatBot: I'm just a bot, but I'm doing great! 😄")
        elif "name" in user_input:
            print("🤖 ChatBot: My name is RuleBot.")
        elif "bye" in user_input:
            print("🤖 ChatBot: Goodbye! Have a nice day!")
            break
        elif "weather" in user_input:
            print("🤖 ChatBot: I can't check live weather, but I hope it's nice outside!")
        elif "time" in user_input:
            from datetime import datetime
            print("🤖 ChatBot: The current time is:", datetime.now().strftime("%H:%M:%S"))
        else:
            print("🤖 ChatBot: Sorry, I don't understand that. Can you rephrase?")

# Run the chatbot
chatbot()
