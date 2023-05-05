# Rest service. JWT server on spring.
This project is intended for learning Rest API and JWT concepts.
The authentication mechanism is as follows
- The API client sends us an object with a username and password.
- If the password matches, then we generate access and refresh tokens and send them in response.
- The API client uses the access token to interact with the rest of our API endpoints.
- Five minutes later, when the access token expires, the front sends a refresh token and receives a new access token. And so on in a circle until the refresh token goes out.
- Refresh token is issued for 30 days. Around day 25-29, the API client sends a valid refresh token along with a valid access token and receives a new pair of tokens in return.

## Table of contents
* [Summary](#summary)
* [Tech Stack](#tech-stack)
* [Environment](#environment)
* [Contacts](#contacts)

## Description
Authorization

## Tech Stack:
- Java: 17
- SpringBoot: 2.7.0
- jsonwebtoken: 0.11.5
- jaxb-api: 2.3.1

## Environment
JDK 17, IntelliJ IDEA CE 2021.3.3, Maven 3.8.1, PostrgreSQL 15

## Contacts
telegram: @knownasmars