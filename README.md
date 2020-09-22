# AI Enterprise Workflow - Capstone Project Submission

My capstone project submission for the IBM AI Enterprise Workflow course on Coursera.

## Usage

Start application.
```bash
python run_app.py
```
Test application.
```bash
python run_tests.py
```
Get result from model (default is total revenue for next 30 days).
```bash
curl --request POST 'http://127.0.0.1/predict?date=2018-11-20'
```
Build image.
```bash
docker build -t app .
```
Run image.
```bash
docker run \
    -it \
    --rm \
    -p 3000:80 \
    --name app \
    app
```

## Endpoints

- `POST /predict?date={date}&duration={duration}&country={country}`
- `POST /logs?type={type}`
