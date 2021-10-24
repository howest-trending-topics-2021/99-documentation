# Clocker

![logo](Assets/logo.png)

## Introduction

---

Clocker is a planning application designed to make telecommuting and on-site work as easy as possible to keep track of. We came up with this idea because Hybrid working is becoming the new norm but in terms of planning and knowing who works where there are not many dedicated programs for that yet.

In Clocker there are two types of users: the Manager and the Employees. The employees are free to fill in their weekly planning so that both the manager and the other employees know who works when. When you schedule a work time you are going to have to indicate if you are going to telecommute or work on-site. This will allow others to know immediately when you will be in your office. And as an extra you will also be able to see the probability that someone will come to work, this probability is calculated by means of an AI.

So the goal is to create a clear planning and clocking in and out system so that there could be less confusion between teleworking and on-site working.

## Technical details

---

### How it works

#### Front-end

---
The clocker application will be accessible by both windows (through native or web app) and mobile devices (through progressive web app). Both front end applications will make api calls to the server to process the necesarry data. to see a preview of the application we made some wireframes:

- [Mobile device](https://www.figma.com/proto/g6TJiAJBRGXMN9jPIClO9B/Trendingtopics?node-id=120%3A4708&scaling=contain&page-id=120%3A4705&starting-point-node-id=120%3A4708)
- [Windows device](https://www.figma.com/proto/g6TJiAJBRGXMN9jPIClO9B/Trendingtopics?node-id=120%3A836&scaling=scale-down&page-id=120%3A2&starting-point-node-id=120%3A836)

if you want to change some things or improve some of the designs the wireframes are available [here](https://github.com/howest-trending-topics-2021/99-documentation/tree/main/Wireframes).

#### Back-end

---
For the server that will be processing the data we use an api for the clients to interact with the server. The API specification is available to see [here](https://github.com/howest-trending-topics-2021/99-documentation/tree/main/API/swagger.yaml).

This is not the only part of the server, we also have an AI part that is going to be created with python and an eventstore. these will also be accessable by api calls but only for the other two servers, to see the diagram on how the servers will be communicating with eachother we made some diagrams [this](https://github.com/howest-trending-topics-2021/99-documentation/blob/main/Diagrams/Container%20Diagram.vsdx) diagram will show you how the front end and back end parts are in connection.

#### Deliverables

---
These are the deliverables for this project:

- front-end pwa
  - employer panel
  - badge system
  - planning system
  - settings page
  - login page
  - no internet connection page
- front-end windows
  - employer panel
  - badge system
  - planning system
  - settings page
  - login page
- back-end
  - badge system
  - planning system
  - employer panel
  - SRP
- database
  - badge system
  - planning systeem
  - employee/employer systeem
- AI
  - Data API
  - AI API
  - Web panel
