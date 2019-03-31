## Introduction

Turkish Deep Learning based Chatbot

The chatbot is implemented on top of RASA stack. You can also run it on your on-premise system. But for now this is only experimental version and not ready for production yet.

What we are doing here then? 
For now, we are updating the NLU data in Turkish language!

## Installation

To install, please clone the repo and run:
```console
$ cd chatbot-tr
$ pip install -e .
```
This will install the bot and all of its requirements. Note that it was written in Python 3 so might not work with PY2.


## Train

For training NLU model, please run:
```console
$ make train-nlu
```

For training Core model, please run:
```console
$ make train-core
```

## Run

Before running chatbot, you shoud run duckling server:
```console
$ docker run -p 8000:8000 rasa/duckling
$ make run-cmdline
```
