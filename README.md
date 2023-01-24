# elearn-gcp

% pwd
/Users/cmyeung/GitHub/elearn-gcp/serverless-python
% pipenv install fastapi uvicorn

% pipenv shell
(serverless-python) % uvicorn main:app --reload

## Run

```
docker build -t serverless-python -f Dockerfile .

docker run --env PORT=5000 -it -p 80:5000 serverless-python
```

## Push

#### via Docker

```
docker build -t serverless-python -f Dockerfile .

docker tag serverless-python grc.io/cloud-test-20221223/serverless-python

docker push grc.io/cloud-test-20221223/serverless-python
```
