# HR Mate - Microsoft Copilot Bot for Employee Task Automation

## Introduction

HR Mate is a Microsoft Copilot bot designed to streamline day-to-day employee tasks directly within Microsoft Teams. Built to enhance productivity and simplify HR-related processes, HR Mate empowers employees to manage personal details, attendance, leaves, timesheets, salary information, company policies, and project management tasks seamlessly. Integrated with notifications and a robust knowledge base, HR Mate ensures employees stay informed and can interact with HR processes efficiently.

## Key features include:

- **Personal Details**: View employee details.
- **Attendance**: Clock in/out, apply for regularization, and view regularization records.
- **Leaves**: Apply for leaves and view leave history.
- **Timesheets**: Submit and review timesheets.
- **Salary**: Access bank details and salary structure.
- **Policies**: Download company policy documents.
- **Manage Projects**: Integrate with DevOps to create/update user stories and tasks.
- **Notifications**: Receive reminders for clock-in/out, upcoming holidays, employees on leave, HR announcements, and query company policies.

## HR Mate leverages the following knowledge base:

- **Dataverse**: For structured employee and HR data.
- **Company Policy Files**: For policy-related queries and downloads.
- **Company Website**: For additional organizational information.

## Technologies used:

- **AI Prompt**: For natural language understanding and responses.
- **Copilot Studio File Search**: For retrieving policy documents and other files.
- **Actions**: To execute specific tasks like clock-in or leave applications.
- **Topics**: To organize conversation flows for various tasks.

This repository contains the configuration and setup details for deploying HR Mate in your organization.

## How to Use HR Mate

### Prerequisites

- A Microsoft 365 subscription with access to Microsoft Teams.
- Access to Power Platform and Copilot Studio for bot configuration.
- A Dataverse environment set up with relevant employee and HR data.
- Company policy files and website content accessible for integration.
- Azure DevOps integration (optional, for project management features).
- Administrative access to configure the bot in Copilot Studio and Teams.

### Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/HappySingh0034/hrmate.git
   cd hr-mate
   ```

2. **Set Up Copilot Studio:**
   - Log in to Copilot Studio.
   - Import the bot configuration files from the copilot-config directory.
   - Configure the bot's connection to Dataverse and file storage for policy documents.

3. **Configure Knowledge Base:**
   - Upload company policy files to a designated storage location (e.g., SharePoint or OneDrive) and link it in Copilot Studio.
   - Ensure the company website URL is added to the bot's knowledge base settings.
   - Validate Dataverse tables for employee data, attendance, leaves, timesheets, and salary details.

4. **Set Up Notifications:**
   - Configure notification triggers in Copilot Studio for:
     - Clock-in reminder at 9:30 AM.
     - Clock-out reminder at 6:30 PM.
     - Daily updates on employees on leave and upcoming holidays.
     - HR announcements.
   - Use Power Automate flows (if needed) to schedule and deliver notifications via Teams.

5. **Integrate with Azure DevOps (Optional):**
   - Set up an Azure DevOps connection in Copilot Studio for project management features.
   - Configure actions to create/update user stories and tasks.

6. **Deploy to Teams:**
   - Publish the bot in Copilot Studio.
   - Add the bot to Microsoft Teams as an app.
   - Assign necessary permissions for employees to interact with the bot.

### Usage

Once deployed, employees can interact with HR Mate in Microsoft Teams by:

1. **Starting a Chat:**
   - Open Teams and search for "HR Mate" in the chat or app section.
   - Initiate a conversation with commands like "View my details," "Clock in," or "Apply for a leave."

2. **Available Commands:**
   - **Personal Details**: "Show my details" or "View my profile."
   - **Attendance**: "Clock in," "Clock out," "Apply regularization," or "View regularization."
   - **Leaves**: "Apply for a leave" or "Show my leave history."
   - **Timesheets**: "Submit timesheet" or "View timesheets."
   - **Salary**: "Show salary details" or "View salary structure."
   - **Policies**: "Download company policy" or "What is the leave policy?"
   - **Manage Projects**: "Create user story," "Update task," or "Show my tasks."
   - **General Queries**: Ask questions like "What is the work-from-home policy?"

3. **Notifications:**
   - Employees will receive automated reminders and updates in Teams, such as clock-in/out prompts, holiday alerts, and HR announcements.

### Customization

- **Add New Topics**: Extend the bot's functionality by creating new topics in Copilot Studio for additional tasks or queries.
- **Update Knowledge Base**: Regularly update policy files and Dataverse records to keep information current.
- **Modify Notifications**: Adjust notification schedules or content in Power Automate or Copilot Studio.

### Troubleshooting

- **Bot Not Responding**: Ensure the bot is published and connected to Teams. Check Copilot Studio logs for errors.
- **Data Issues**: Verify Dataverse table permissions and data accuracy.
- **Notification Failures**: Confirm Power Automate flows are active and correctly configured.
- **DevOps Integration Errors**: Validate Azure DevOps credentials and API permissions.

## Contributing

Contributions are welcome! Please fork the repository, make your changes, and submit a pull request. Ensure your code follows the repository's coding standards and includes relevant documentation.

