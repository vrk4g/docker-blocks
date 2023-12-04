FROM python
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1
ARG REQ_POSTFIX
COPY ./req_${REQ_POSTFIX}.txt ./
RUN pip install --upgrade pip
RUN pip install -r req_${REQ_POSTFIX}.txt
WORKDIR /app
COPY ./app ./