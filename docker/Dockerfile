FROM python:3-alpine

RUN pip install --root-user-action ignore --upgrade pip 
COPY requirements.txt /tmp
RUN pip install --root-user-action ignore -r /tmp/requirements.txt
COPY app /opt/japp

USER 1000
ENTRYPOINT ["python", "/opt/japp/app.py"]
