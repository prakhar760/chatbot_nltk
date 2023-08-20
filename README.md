# Chatbot Deployment with Flask and JavaScript

## Initial Setup:

Clone repo and create a virtual environment
```
$ git clone https://github.com/python-engineer/chatbot-deployment.git
$ cd chatbot-deployment
$ python3 -m venv venv
$ source venv/bin/activate
```
Install dependencies
```
$ (venv) pip install Flask torch torchvision nltk
```
Install nltk package
```
$ (venv) python3
>>> import nltk
>>> nltk.download('punkt')
```
Modify `intents.json` with different intents and responses for your Chatbot

Run
```
$ (venv) python3 train.py
```
This will dump data.pth file. And then run
the following command to test it in the console.
```
$ (venv) python3 chat.py
```
Run the Flask app.
```
$ (venv) python3 app.py
```
## Note
In the video we implement the first approach using jinja2 templates within our Flask app. Only slight modifications are needed to run the frontend separately. I put the final frontend code for a standalone frontend application in the [standalone-frontend](/standalone-frontend) folder.

## Credits:
This repo was used for the frontend code:
https://github.com/hitchcliff/front-end-chatjs
