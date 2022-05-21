

# Abstractive Text Summarization API



Automatic text summarization comprises a set of techniques that use algorithms to condense a large body of text, while at the same time preserving the important information included in the text. It is an area of computer automation that has seen steady development and improvement, although it does not get as much press as other machine learning achievements.
Automatic summarization as a field is not limited to text. In fact, we can 'summarise' images and videos as well as text. Wikipedia defines automatic summarization as "the process of shortening a set of data computationally, to create a subset (a summary) that represents the most important or relevant information within the original content". The end goal, whether we summarise text, images or videos, is to reduce the number of resources required to transmit and process data.
If we exclude human assisted solutions, we generally have two main approaches to automatic text summarization:
- Extractive summarization
- Abstractive summarization

Extractive summarization algorithms perform a seemingly very simple task: It takes in the original text document and extracts parts of it that it deems important. This means that it do not create new data (new sentences). Instead, these models simply select parts of the original data which are most important and combine them to form a summary.
This contrasts with how most humans summarize text. Instead of simply copying over the most important sentences, a well written summary authored by a human will contain new sentences which include just the most important points in the original text. Fortunately, we do have models that work in a similar fashion.


This project implements abstractive text summarization using an API built in flask. The program uses a pre-trained model named Pegasus to create abstractive text Summary. 



## Installation

To set up the this project you can directly download all the dependencies using the reqirements.txt 

```bash
  pip install -r /path/to/requirements.txt
```

or you can indivisually download all the dependencies

```bash
    pip install torch
    pip install flask
    pip install sentencepiece
    pip install transformers
    pip install flax
    pip install --upgrade tensorflow
```

to check if tensorflow is installed correctly or not you can run the following command

```bash
    python -c "import tensorflow as tf;print(tf.reduce_sum(tf.random.normal([1000, 1000])))"
```
## Run Locally

- Clone the project

```bash
  git clone https://github.com/aditya-gitte/Abstractive-Text-Summarization-API.git
```

- Go to the project directory



- Create a new virtual environement and install all the dependencies

- Set the Flask environment variable using
```bash
  set FLASK_APP=app.py
  $env:FLASK_APP = "app.py"

```

- Start the server by either manually running the `app.py` file or using 

```bash
  flask run
```
- The test server will run on http://127.0.0.1:5000/ by default

- Pass the text whose summary has to be found in the url bar after '/' (http://127.0.0.1:5000/Sample_text_whose_summary_has_to_be_found)

- Since the code is compute heavy wait for 2-3 minutes for execution. For the first time it will take even longer as a 2.5GB model has to be downloaded and cached Locally.



