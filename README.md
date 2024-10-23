# Jenkins Pipeline Project

This project demonstrates how to set up a Jenkins pipeline that triggers automatically when changes are pushed to this repository.

## How it works

1. The repository is connected to Jenkins through a webhook (configured using ngrok).
2. The `Jenkinsfile` defines the steps for building and deploying the code.
3. Any change to the `main` branch will trigger the pipeline automatically.

## Steps to configure

- Add this repository URL to Jenkins.
- Configure a webhook using ngrok to connect Jenkins to Git.

