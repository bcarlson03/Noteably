# Noteably - HackKU23 Project

This is a project created for HackKU23 created by Blake Carlson, Michael Stang, Holden Vail, and Logan Smith. 

Noteably is an AI-Powered Note taking tool that can automate the note-taking process. Simply give it an audio file of a lecture, meeting, seminar, or more, and it will automatically create refined notes and full transcriptions to create a more accessible learning environment and elevate the learning oppurtunities for those who may be unable to take notes or those who find taking notes distracting. 

Installing Noteably is very simple. Start by cloning this GitHub repo as seen below.

```
git clone git@github.com:bcarlson03/HackKU23-Project.git
```


Once it is installed, simply run the following command while located at the repo to install all needed packages for Notebly to run. 

```
python -m pip install -r requirements.txt
```

Once installed, using Noteably is quite simple. After your first run of "main.py" two folders will be created, "audio_files" and "notes." Place all of your .wav files in the "audio_files" folder and run the program to start the process.

After intalling all of the normal and setting up the majority of the functions for the program there is still one small step that you will need to take to get your copy of Noteably up and running. Noteably uses a cloud based implementation of google's speech-to-text API as well as their cloud storage API. One of the limitations of using these APIs is that you will need to enroll for a verified google developer account. After registering you will also need to install and enable your programs to run within thier framework. They offer some excellent instructions which you can find here: 

https://cloud.google.com/sdk/docs/install

Following the successful installation of the necessary resources, you will be start the program in one of two ways...

You can run "main.py" to simply convert the .wav files in the folder into .pdfs in the "notes" folder. If you would like a more guided experience, run "interface.py" to open an interactive GUI which can add files from anywhere on your device. Then click "Generate" to start the conversion process.

This project is powered by Google Cloud's API to allow for rapid speech-to-text conversion. It also leverages OpenAI's GPT Davinci-002 model for note refinement.
