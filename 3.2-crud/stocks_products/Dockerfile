FROM python:3.9

COPY ./requirements.txt /src/requirements.txt

RUN pip3 install --no-cache-dir --upgrade -r /src/requirements.txt

COPY . /src

EXPOSE 8765

WORKDIR src

ENV SECRET_KEY jango-insecure-nw^y+m^wmxza1asgk+)!ua2qx9)g+#v=6%76-9i8i(6eqiw94j
ENV DEBUG True

RUN python manage.py migrate

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]