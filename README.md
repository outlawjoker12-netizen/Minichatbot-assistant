# Minichatbot-assistant
Very simple chat bot 
# mini assistant chatbot
print("welcome to your smart assistant")  # welcome statement
name = input("hello! your name is? ")    #ask for name 

#define greeting
def greet( ):
	print("hello,", name)
	return name

#chatbot responses
def assistant_response(command):
	if command == "hello":
		print("Hello! im your assistant.", "what can I help with?", user_name)
	elif command == "time":
		print("I can't tell time yet, but i will soon")
	elif command == "help":
		print("Commands: hello, time, help, quit")
	else:
			print("sorry i don't understand, I am still learning.")
user_name = greet( )     #stores greet function in user_name variable 

   #starts the loop funcion
while True:
	user_command = input(">>> ").lower()   #(>>> ).lower() allows user input and lowercases whats inside
	if user_command == "quit":
		print(f"Goodbye, {user_name} !")
		break
	assistant_response(user_command)    #must be inside while loop inorder to execute 
