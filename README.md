# Deploy FastAPI dengan menggunakan App Engine
Deploy FastAPI dengan menggunakan App Engine


## Kebutuhan
* Pyenv (optional)
* Virtualenv (optional)
* Python 3.8.2
* Google Cloud Platform Account
* Google Cloud Platform - API Cloud Build


## Jalankan secara lokal
```
$ virtualenv -p python3.8.2 .venv
$ source .venv/bin/activate
$ pip install -r requirements.txt
$ gunicorn -w 4 -k uvicorn.workers.UvicornWorker main:app
```

## Cara deploy ke app-engine
```
$ gcloud app create
$ gcloud app deploy app.yaml --project <project_id>
$ gcloud app browser
```
