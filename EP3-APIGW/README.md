# Serverless Office Hours: Amazon API Gateway - transforming API requests and responses in HTTP APIs

In this episode, we demonstrate transforming API requests and responses with Amazon API Gateway HTTP APIs and then open up the last half to help you with your serverless challenges and issues.

[View on YouTube](https://youtu.be/wuBt3N6wa2s)

## Requirements
* [AWS SAM CLI](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-install.html)
* An account with [Open Weather Map](openweathermap.org)

## Setup
Create am AWS Secrets Manager key called *WeatherApiKey* with your open wather API key in it

## Deploying
```bash
sam deploy
```