FROM python:3.8-alpine

RUN apk --no-cache add gcc make musl-dev libffi-dev openssl-dev

RUN pip install awscli

RUN apk --no-cache del gcc make musl-dev libffi-dev openssl-dev
