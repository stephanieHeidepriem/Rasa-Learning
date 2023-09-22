# Introduction 
Learning Projects

# Getting Started
## Prerequisites:
- Visual Studio Build Tools are installed (https://visualstudio.microsoft.com/de/visual-cpp-build-tools/)
- Python 3.8.0

## Install all dependencies in the virtual environment:
- Create the virtual environment: ```python -m venv ./env``` oder (because older version is needed) ```virtualenv --python="C:\Users\steph\AppData\Local\Programs\Python\Python38\python.exe" "venv"```
 --> you can also change the name to the environment. But make sure, that you don't commit it to the repository
- Enable the virtual environment: ```.\env\Scripts\activate```
- check if pip version is up to date: ```python -m pip install --upgrade pip```
- install all requirements: ```pip install -r requirements.txt```

## Train and run chatbot locally
- Train NLU and Core with: ```python -m rasa train```
- Start Action Server: ```python -m rasa run actions```
- Start Rasa Core (in new Terminal): ```rasa run -m models --enable-api --cors="*"```
- Locally you can check the bot, with opening file:///D:/Repos/Coronachatbot/index.html in Browser

## Run Tests
--> No Tests avalable yet. Only a prototype

## Create Requirements.txt
```pip freeze > requirements.txt```