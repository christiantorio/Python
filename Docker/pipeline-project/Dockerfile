FROM python:3.7.3-stretch

## Step 1:
WORKDIR /app

## Step 2:
RUN pip install -r requirements.txt
RUN hadolint --ignore DL3013 Dockerfile

## Step 3:
COPY . app.py /app/

## Step 4:
EXPOSE 80

## Step 5:
# Run app.py at container launch
CMD ["python", "app.py"]