FROM jenkins/jenkins
LABEL maintainer="Jenkins"

USER root

RUN apt-get update && apt-get install -y bash git curl python3 build-essential libssl-dev libffi-dev python-dev python-pip && rm -rf /var/lib/apt/lists/*

RUN pip install ansible \
    aws \
    boto \
    boto3

RUN pip install awscli --upgrade

USER jenkins
