
# Surveykshan Research Data Collection App

## Overview

The **Surveykshan Research Data Collection App** is a Kotlin-based Android application designed for efficient data collection and survey management. The app allows team members to authenticate, access survey forms, fill out various types of questions, and submit responses. It integrates various APIs, background tasks, and cloud storage for file handling to streamline the data collection process.

This project is a migration from Java to Kotlin and utilizes modern Android components and libraries like **Retrofit**, **Volley**, **Coroutines**, **Firebase Crashlytics**, and **AWS** for a more optimized and scalable solution.

## Features

### Key Functionalities:

- **Team Login API**: Secure login for team members.
- **Registration API**: User registration for joining the survey team.
- **Survey Form List API**: Fetches available survey forms to be filled out.
- **Submit Response API**: Submits the filled-out responses to the server.
- **Dashboard API**: Displays important metrics and details:
  - Surveys taken today
  - Total surveys conducted
  - Device model and file responses
  - User and team details

### Questionnaire Form Types:

- **MCQ (Multiple Choice Questions)**
- **Matrix Type Questions (Radio, Checkbox, Input fields)**
- **Contact Information**
- **File Upload (Images, Audio, Recordings)**
- **Short Text**
- **Long Text**
- **Statement**
- **Dropdown**
- **Rating**
- **Checkbox**

### File Handling:
- Text responses are stored and sent as JSON data to the server.
- File responses (images, recordings, audio) are uploaded to **AWS** cloud storage.

### Background Tasks:

- **WorkManager** is used to automatically update local data in the background.
- Notifications with low importance are used to inform users about completed tasks.

### Error Tracking:
- **Firebase Crashlytics** is integrated to track and log app crashes and exceptions in real time.

## Tech Stack

- **Programming Language**: Kotlin
- **API Integration**: Retrofit, Volley
- **Asynchronous Programming**: Coroutines
- **Background Task Handling**: WorkManager
- **Error Logging**: Firebase Crashlytics
- **Cloud Storage**: AWS
- **UI Components**: Android Views, Custom UI for different question types
- **Data Storage**: JSON format for responses

