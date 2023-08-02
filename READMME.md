# Set-Up

# Virtual Environment
Create a new virtual environment
`$ venv venv`

Activate virtual environment
`$ . venv/bin/activate`

# Python packages

Install the dependencies written in requirements.txt

`$ pip install -r requirements.txt`

# Train

Run the script in code/train.py, this script takes the input data and outputs a trained model and a pipeline for our web service.

`$ python code/train.py`

# Web application

Test web app:

`$ flask run -p 5000`

# Docker

Use Dockerfile to create image for running web app inside a container

`$ docker build . -t from_ds_to_mlops`

Test app using Docker

`$ docker run -p 8000:8000 from_ds_to_mlops`

# Test

Test calls in tests/example_calls.txt