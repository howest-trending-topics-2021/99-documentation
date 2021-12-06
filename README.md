# Clocker

![logo](Assets/logo.png)

## Introduction

---

Clocker is a planning application designed to to keep track of telecommuting and on-site work. We came up with this idea because Hybrid working is becoming the new norm but in terms of planning and knowing who works where there are not many dedicated programs for that yet.

In Clocker there are two types of users: the Manager and the Employees. The employees can fill in their weekly planning so both the manager and the other employees know who works where and when. When you schedule a work time you are going to have to indicate if you are going to telecommute or work on-site. This will allow others to know immediately when you will be in your office. And as an extra you will also be able to see the probability that someone will come to work, this probability is calculated by means of an AI.

So the goal is to create a clear planning and clocking system so that there could be less confusion between teleworking and on-site working.


## Technical details

---

### How it works

---

The application consists of several deployables that need to be rolled out seperately.  

#### PWA

---

The Progressive Web App is the user interface that has been developed to access the application from a mobile device. 
The application allows the user to 
* add his schedule for the week
* check the schedule of his collegues
* monitor his performance
* check and change the settings

A demo application has been set up at: https://kind-mud-02e3e2c03.azurestaticapps.net/ (username/password: manager/manager)

To deploy a new version of the application, all information can be found [here](https://github.com/howest-trending-topics-2021/01-frontend-web)



#### Desktop App

---

The desktop application is an identical interface as the PWA, but is intended to run on a native Windows environment such as a laptop or desktop.

A demo application has been build and can be downloaded from [here](https://studenthowest-my.sharepoint.com/:u:/g/personal/kwinten_tas_student_howest_be/Ed2ai3dnFtdBrtyH5yh0GcQBZoKwRNSjCZd012c5ClO0Wg?e=h2UzCW)

To build a new version, all information can be found [here](https://github.com/howest-trending-topics-2021/01-frontend-web)

#### Backend Server

---

The business logic has been contained in the Backend Server. 

The available endpoints from the demo server can be consumed through [this API specification](https://github.com/howest-trending-topics-2021/99-documentation/tree/main/API/swagger.yaml)

To deploy a new server, redirect to [this link](https://github.com/howest-trending-topics-2021/02-backend)

#### AI Server

---

One specific part of the business logic is the prediction if an employee is likely to come in. This prediction is done by the AI server.

To deploy another AI server, go to [this repo](https://github.com/howest-trending-topics-2021/05-AI) for all information

#### Database

---

All data has to be preserved in a database. For this project we made use of an Datahike eventstore.

A demo database has been deployed to support the demo server, but this one is not publicly available.

To deploy your own database, read the instructions [here](https://github.com/howest-trending-topics-2021/03-database)


