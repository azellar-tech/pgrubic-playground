FROM python:3.13-slim@sha256:6544e0e002b40ae0f59bc3618b07c1e48064c4faed3a15ae2fbd2e8f663e8283

WORKDIR /src

COPY app app

COPY requirements.txt requirements.txt

RUN pip install --no-cache-dir --upgrade pip -r requirements.txt

# Switch to non-root user.
USER 10001

CMD ["python3", "app/main.py"]
