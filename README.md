# TalkWithAI
This is a simple project that allows you to basically converse with any person/object/character by using GPT API. This project uses ChatGPT API and ElevenLabs API to generate text and speech respectively.
It follows a simple 3 step approach.
### 1.Speech to Text (STT)
In this step, the audio input from the user's speech is converted into text using speech recognition technology. Due to lack of freely available/cheap real time transcribing, we first save the audio in a .wav file and then apply the transcribing on the audio file using Whisper API(or you may also run Whisper on your local machine but might delay the transcribing depending on CPU/GPU). The STT system analyzes the spoken words, translates them into written text, and provides a textual representation of the user's speech.
### 2.Text to Text (TTT)
Once the user's speech has been converted into text, the TTT step processes the text input and generates a suitable response or action based on the user's query or command. This involves utilizing ChatGPT API that gives a suitable response so as to continue the conversation as expected.
### 3.Text to Speech (TTS)
Finally, in the TTS step, the generated textual response is converted back into spoken language using text-to-speech synthesis. The TTS system takes the text response and produces an audio output that can be understood by the user, allowing for a natural conversation-like interaction between the user and the AI system.We are using the ElevenLabs API to generate Speech because it allows you to create different voices with accents or choose a voice from a vast Voice Library.

## Prerequisites
* Python >= 3.5
* an OpenAI API key
* an ElevenLabs API key

## Setup
You may either run the following command in terminal 

`$ pip install -r requirements.txt`

Or you may alternatively install all the packages in the file `requirement.txt`.

## Installation
1. Clone this repository.
2. Go to TalkwithCeleb.Py and add your OPENAI_API key and ElevenLabs_API key.
3. Select the appropriate Voice ID from Voice Library of ElevenLabs and replace it with the Voice ID.
4. Run the file and start talking.
