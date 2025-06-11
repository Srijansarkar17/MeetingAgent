# MeetStream AI - Meeting Assistant
Introducing your ultimate meeting assistant: it records your meetings, transcribes them in real-time, identifies tasks, auto-sends personalized emails to each team member, and even schedules follow-ups directly on Google Calendar. Save time, stay organized, and let this agent do the heavy lifting.

## ⚠️ Project Status

**This is an ongoing project and is not yet fully completed.** 

Some features may be in development or require additional configuration. Please check the issues section for known limitations and upcoming features.

---

## Project Overview

MeetStream AI is your ultimate meeting assistant that revolutionizes how you handle meetings and follow-ups. This intelligent system:

### Key Features:
- **🎙️ Real-time Meeting Recording** - Automatically records and transcribes your meetings
- **🤖 Smart Task Detection** - Uses AI to identify tasks and action items from transcripts
- **📧 Automated Email Notifications** - Sends personalized task assignments to team members
- **📅 Calendar Integration** - Automatically schedules follow-up meetings on Google Calendar
- **💬 Slack Integration** - Sends task notifications via Slack messages
- **👥 Contact Management** - CSV-based contact system for easy team management

### How It Works:
1. **Meeting Recording**: The bot joins your meeting and records the conversation
2. **AI Processing**: Groq AI analyzes the transcript to extract tasks and scheduling intents
3. **Smart Matching**: Uses intelligent name matching to find team members in your contacts
4. **Multi-channel Notifications**: Sends tasks via both email and Slack
5. **Calendar Scheduling**: Automatically creates calendar events for follow-up meetings

---

## Technologies Used

### Backend & Core
- **Flask** - Web framework for API endpoints
- **Python** - Primary programming language
- **Groq AI** - AI processing for transcript analysis and task extraction
- **Google APIs** - Calendar integration and Gmail services
- **Slack SDK** - Slack messaging integration

### AI & Data Processing
- **Groq AI** - Natural language processing for meeting transcripts
- **Pandas** - Data manipulation for contacts management
- **OpenAI** - Additional AI capabilities
- **Tavily Python** - Web search functionality
- **DuckDuckGo Search** - Alternative search integration

### Google Services Integration
- **Google Calendar API** - Automatic event scheduling
- **Gmail API** - Email notifications and task assignments
- **Google Auth** - OAuth2 authentication flow

### Web Automation & Scraping
- **Selenium** - Web automation
- **WebDriver Manager** - Browser driver management
- **BeautifulSoup4** - HTML parsing
- **python-docx** - Document processing

### Utilities
- **python-dotenv** - Environment variable management
- **Requests** - HTTP client for API calls
- **Pickle** - Credential storage

---


## Installation and Setup Guide

### Prerequisites
- Python 3.8+
- Google Cloud Console account
- Groq AI API key
- Slack Bot Token (optional)

### 1. Clone the Repository
```bash
git clone <repository-url>
cd meetstream-ai
```
### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Environment Setup
- Create a .env file in the project root:
```bash
GROQ_API_KEY=your_groq_api_key_here
SLACK_BOT_TOKEN=your_slack_bot_token_here
CONTACTS_CSV=path_to_your_contacts.csv
BOT_ID=will_be_auto_generated
```

### 4. Google API Setup
- Go to Google Cloud Console
- Create a new project or select existing one
- Enable Google Calendar API and Gmail API
- Create credentials (OAuth 2.0 Client ID)
- Download the credentials and save as credentials.json in project root

### 5. Contacts CSV Setup
- Create a CSV file with the following columns:
```bash
name,email,slack_id
John Doe,john@example.com,U1234567890
Jane Smith,jane@example.com,U0987654321
```
### 6. Slack Bot Setup (Optional)
- Go to Slack API
- Create a new app
- Get the Bot User OAuth Token
- Add it to your .env file

### 7. Run the Application
```bash
python app.py
```
---

## Contact Me

### Connect with me on social media:

**Twitter**: [@srijan4ai](https://x.com/srijan4ai)

**LinkedIn**: [Srijan Sarkar](https://www.linkedin.com/in/srijan-sarkar-90177b288/)

---

*Feel free to contribute to this project or report any issues you encounter!*

