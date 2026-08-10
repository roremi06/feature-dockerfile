FROM python:3.12-slim

# setup work directory
WORKDIR /app

# copy requirements to work directory
COPY requirements.txt .

# install requirements
RUN pip install --no-cache-dir -r requirements.txt

# copy what we have from local folder to work directory
COPY . .

# expose the port on which the app will run
EXPOSE 8005

# run app
CMD ["fastapi", "dev", "src", "--host", "0.0.0.0", "--port", "8005"]