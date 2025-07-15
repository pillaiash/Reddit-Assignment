# Reddit-Assignment

Reddit User Persona Generator
Project Overview
This script generates a detailed user persona by analyzing a Reddit user's profile. It scrapes their recent posts and comments, uses an AI model to create a persona with characteristics and interests, and cites the specific sources for each insight. This project was completed as part of the AI/LLM Engineer Intern assignment for BeyondChats.
Features
Scrapes recent posts and comments from any public Reddit user profile.
Uses a Large Language Model (LLM) via OpenRouter to analyze the user's activity.
Generates a detailed user persona, including demographics, interests, and personality traits.
Provides direct URL citations for every piece of information in the persona.
Saves the final persona to a .txt file.
Setup and Installation
Prerequisites
Python 3.8 or newer
A Reddit account
An OpenRouter.ai account
1. Clone the Repository
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name


2. Install Dependencies
This project requires a few Python libraries. Install them using pip:
pip install praw openai==0.28 requests


3. Set Up Credentials
The script needs API keys to connect to Reddit and OpenRouter. You need to add your credentials to the persona_analyzer.py script.
Important: Do not commit your secret keys directly to your public GitHub repository.
Create a Reddit Script App:
Go to your Reddit app preferences.
Click "are you a developer? create an app..."
Name your app, select "script" as the type, and set the redirect URI to http://localhost:8080.
You will get a client id and a client secret.
Get an OpenRouter API Key:
Sign up or log in at OpenRouter.ai.
Go to your Keys page to get your API key.
Add Credentials to the Script:
Open the persona_analyzer.py script.
Find the credentials section at the top and replace the placeholder values with your actual keys.
How to Execute the Script
To analyze a new Reddit profile, run the script from your terminal and provide the user's profile URL as an argument.
python persona_analyzer.py <reddit_profile_url>


Example:
python persona_analyzer.py https://www.reddit.com/user/Google/


Output
The script will generate a text file named <username>_persona.txt in the same directory. This file contains the complete user persona with citations.
Included Sample Outputs
As per the assignment requirements, this repository includes the pre-generated persona files for the two sample users:
kojied_persona.txt
Hungry-Move-6603_persona.txt
