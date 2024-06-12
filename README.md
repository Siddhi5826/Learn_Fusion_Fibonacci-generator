Python code for Voice Assitant
Install the necessary libraries:
speech_recognition for converting speech to text.
pyttsx3 for text-to-speech conversion.

pip install speechrecognition pyttsx3

Explanation:
Initialization:

recognizer = sr.Recognizer(): Initializes the speech recognizer.
tts_engine = pyttsx3.init(): Initializes the text-to-speech engine.
Speak Function:

speak(text): Converts the given text to speech using pyttsx3.
Listen Function:

listen(): Listens for audio input from the microphone and converts it to text using Google Web Speech API.
Process Command Function:

process_command(command): Processes the recognized command and executes appropriate actions (e.g., responds to greetings, provides its name, or exits).
Main Function:

main(): The main loop of the voice assistant that listens for commands and processes them continuously until the user says "exit".
This is a basic implementation. In a real-world scenario, you would want to add more error handling, support for more commands, and possibly integrate with other APIs or services to enhance the assistant's capabilities.

Python code for Fibonacci generator, in this 
def fibonacci_generator():
    a, b = 0, 1
    while True:
        yield a
        a, b = b, a + b

# Usage example:
fib_gen = fibonacci_generator()
for _ in range(10):
    print(next(fib_gen))
    
