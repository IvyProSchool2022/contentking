# Doctor-Bot: AI Medical Chatbot

Doctor-Bot is an AI-powered chatbot designed to provide general health advice and guidance on common ailments, symptoms, and emergency situations. The app is built with Flask for the backend and HTML/CSS/JavaScript for the frontend, utilizing OpenAI's GPT API for natural language processing.

## Table of Contents
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Setup and Installation](#setup-and-installation)
- [Environment Variables](#environment-variables)
- [Deployment on Railway](#deployment-on-railway)
- [Project Structure](#project-structure)

---

## Features

- **Health Advice**: Provides general health advice and guidance on common ailments.
- **Symptom Checker**: Offers suggestions based on reported symptoms.
- **Emergency Guidance**: Supplies advice for emergency situations like burns or CPR.
- **Interactive Chat Interface**: Communicates with users in real-time with typing effects.

---

## Tech Stack

- **Backend**: Flask, Python
- **Frontend**: HTML, CSS, JavaScript
- **API**: OpenAI's GPT API (for generating responses)
- **Hosting**: Railway.app

---

## Setup and Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/doctor-bot.git
cd doctor-bot
```

### 2. Install Dependencies

Ensure you have Python installed. Then, install the dependencies using:

```bash
pip install -r requirements.txt
```

### 3. Environment Variables

To connect to OpenAI’s API, you'll need an API key. Set up your environment variables as follows:

1. Go to [OpenAI](https://platform.openai.com/) and get your API key.
2. Add the `OPENAI_API_KEY` to your environment variables.

For Railway, you can add the key as an environment variable in the dashboard (explained below).

---

## Deployment on Railway

### 1. Connect Your GitHub Repository to Railway

1. Log in to [Railway.app](https://railway.app/) and create a new project.
2. Choose "Deploy from GitHub" and select your Doctor-Bot repository.

### 2. Configure Environment Variables on Railway

1. Go to the **Settings** tab of your Railway project.
2. Under **Environment Variables**, add `OPENAI_API_KEY` with your actual OpenAI API key.

### 4. Deployment

Railway will automatically deploy your application after connecting to your GitHub repository. Check the **Deployments** tab and **Logs** to monitor the deployment process.

---

## Project Structure

- `app.py`: Main Flask app handling requests and responses.
- `templates/index.html`: The HTML file for the frontend interface.
- `static/`: Directory for static files like `favicon.ico` and additional assets.
- `requirements.txt`: Lists project dependencies for Python.
