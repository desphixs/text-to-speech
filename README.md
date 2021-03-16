# text-to-speech
# Text to Speech App with python 4 lines of code

import pyttsx3

talk = pyttsx3.init()
voice = talk.getProperty("voices")
talk.setProperty("voice", voice[1].id)
speech = input("Say something: ")
talk.say(speech)
talk.runAndWait()
