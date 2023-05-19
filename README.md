# Deploy FastAPI dengan menggunakan App Engine
Deploy FastAPI dengan menggunakan App Engine


## Prerequisites
* Pyenv (optional)
* Virtualenv (optional)
* Python 3.8.2
* Google Cloud Platform Account
* Google Cloud Platform - API Cloud Build


## Running Local
```
$ virtualenv -p python3.8.2 .venv
$ source .venv/bin/activate
$ pip install -r requirements.txt
$ gunicorn -w 4 -k uvicorn.workers.UvicornWorker main:app
```

## Deploy Production
```
$ gcloud app create
$ gcloud app deploy app.yaml --project <project_id>
$ gcloud app browser
```
