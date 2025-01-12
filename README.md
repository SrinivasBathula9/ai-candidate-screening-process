# AI-Powered Recruitment Team

This Streamlit application emulates the functionality of a comprehensive recruitment team, utilizing multiple AI agents to automate and enhance the hiring process. Each agent embodies a specific recruitment role—spanning resume screening, candidate evaluation, interview scheduling, and communication—collaborating seamlessly to deliver end-to-end hiring solutions. The system integrates the expertise of technical recruiters, HR coordinators, and scheduling specialists into a unified automated workflow.

## Key Features

#### AI-Powered Agents

- Technical Recruiter Agent: Examines resumes and assesses technical qualifications.
- Communication Agent: Manages email correspondence with candidates.
- Scheduling Coordinator Agent: Oversees interview scheduling and coordination.
- Collaborative Expertise: Each agent specializes in a specific function and works together for a smooth recruitment experience.


#### Streamlined Hiring Process
- Automated resume review and skill analysis.
- Role-specific technical assessments.
- Professional and timely communication.
- Automatic interview scheduling.
- Feedback management and tracking.

## Prerequisites

Before running the application, complete the following:

# Gmail Setup:

- Create or use a Gmail account for the recruiter.
- Enable 2-Step Verification and generate an App Password.
- The App Password is a 16-character code (e.g., afecwejfawojfwrv - remove spaces before entering it). Follow the steps here: Google App   Password.

# Zoom Setup:

- Create or use a Zoom account and navigate to the Zoom App Marketplace.
- Create a new app with the Server-to-Server OAuth option and obtain these credentials:
- Client ID
- Client Secret
- Account ID
# Add the following scopes to enable meeting link creation and communication:
- meeting:write:invite_links:admin
- meeting:write:meeting:admin
- meeting:write:meeting:master
- meeting:write:invite_links:master
- meeting:write:open_app:admin
- Optional scopes:
- user:read:email:admin
- user:read:list_users:admin
- billing:read:user_entitlement:admin
- dashboard:read:list_meeting_participants:admin

## Steps to Launch

1. **Setup Environment**
   ```bash
   # Clone the repository
    git clone https://github.com/SrinivasBathula9/ai-candidate-screening-process.git

   # Install dependencies
   pip install -r requirements.txt
   ```

2. **Configure API Keys**
   - OpenAI API Key for GPT-4 access.
   - Zoom API credentials (Account ID, Client ID, Client Secret).
   - Gmail App Password for the recruiter’s email.

3. **Run the Application**
   ```bash
   streamlit run app.py
   ```

## Core Components

- **Resume Analyzer:**
  - Matches skills and qualifications.
  - Verifies candidate experience.
  - Provides technical evaluations and selection recommendations.
- **Email Communication Manager:**
  - Drafts professional emails.
  - Sends automated notifications.
  - Manages feedback exchanges.
  - Handles follow-ups.
- **Interview Scheduler:**
  - Coordinates Zoom meetings.
  - Manages calendars.
  - Handles time zone differences.
  - Sends reminders to participants.
- **Candidate Experience:**
  - User-friendly resume upload interface.
  - Real-time feedback and updates.
  - Transparent and efficient communication.
## Technical Overview
  - Framework: Streamlit and Phidata.
  - AI Model: OpenAI GPT-4.
  - Integrations: Zoom API, Phidata's EmailTools.
  - PDF Handling: PyPDF2.
  - Time Zone Management: pytz.
  - State Management: Streamlit Session State.
## Important Notes
This tool supports recruitment automation but is not a substitute for human judgment. Always review automated decisions before finalizing hiring outcomes.

## Planned Enhancements
Integration with Applicant Tracking Systems (ATS).
Advanced scoring for candidates.
Video interview functionality.
Comprehensive skills assessment tools.
Multi-language support for global recruitment.
