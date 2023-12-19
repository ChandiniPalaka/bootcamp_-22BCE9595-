# bootcamp_-22BCE9595-
# Creating A ChatBot Using Conditional Statements and loops!

a = input("Hey! What's your name : ")
def chatbot():
    print("YO!"+a+" I'm your ChatBot")
    
    while True:
        b = input("You: ").lower()  # Convert user input to lowercase for case-insensitivity
        
        # Exit the chatbot if the user types 'exit'
        if b.lower() in ['bye', 'exit', 'quit']:
            print("Chatbot: Well! Come back soon for more creative chats!")
            break
        
        # Responding based on user input
        if 'color' in b.lower():
            print("Chatbot: What's your favorite color?")
            color = input("You: ")
            print(f"Chatbot: Ah, {color} is a fantastic choice! It reminds me of a magical rainbow.")

        elif 'sing a song' in b.lower():
            print("Chatbot: 🎶 La, la, la! I'm singing in binary, 0101010101... 🎶")
            
        elif 'how are you' in b:
            print("Chatbot: My mood is as unpredictable as a random number generator!")
           
        elif 'weather' in b:
            print("Chatbot: I'm sorry, I don't have real-time information. You can check a weather website.")
        
        else:
            print("Chatbot: I didn't understand that. Can you ask something else?")

# Run the chatbot
chatbot()
