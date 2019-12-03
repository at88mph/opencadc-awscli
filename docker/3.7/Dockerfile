FROM python:3.7-alpine

RUN apk --no-cache add gcc make musl-dev libffi-dev openssl-dev groff

RUN pip install awscli

RUN apk --no-cache del gcc make musl-dev libffi-dev openssl-dev
