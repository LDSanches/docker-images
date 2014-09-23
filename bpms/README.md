# EAP Domain Docker Image

EAP Version: 6.3

JON Version: 3.2

## build.sh
Use to build EAP Domain docker image.
This image is based on centos 6.
Before building this image, you must download `jboss-eap-6.3.0.zip` and `rhq-enterprise-agent-4.9.0.JON320GA.jar` and put them in software folder.

## runBash.sh
Create a new EAP Domain container running /bin/bash

## runSSH.sh
ssh into your running container.

password: redhat

## runDocker.sh
Create a new container running EAP Domain and JON Agent.

### EAP
After running, you can access EAP Console on your localhost:9990.

User: admin

Password: redhat@123

EAP folder: /opt/jboss/eap

JON agent folder: /opt/jboss/jon

### JON Agent
There is a jon agent running inside this container. It will try to connect to jon-server. So, it is mandatory to start first jon-server container so docker can link with it.