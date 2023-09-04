FROM python:alpine
COPY . /app
WORKDIR /app
RUN pip install -r requirements.txt
RUN addgroup -S myappgroup && adduser -S myappuser -G myappgroup
USER myappuser
EXPOSE 80
CMD python ./phonebook-app.py