FROM apache/airflow:2.9.3-python3.10

WORKDIR /app

# COPY requirements.txt /app/requirements.txt
# В связи с возможной проблемой в неявных зависимостях советую использовать .lock
COPY requirements.lock /app/requirements.lock

RUN pip install --upgrade pip
#RUN pip install --no-cache-dir -r requirements.txt
RUN pip install --no-cache-dir -r requirements.lock