# Power Automate Flow - Daily Task Automation

## Overview:
This Power Automate flow automates routine tasks based on the current day of the month, improving efficiency and communication within the organization.

## Trigger:
- Recurrence: Daily at 12 PM

## Conditions and Actions:

### If the current day is the 15th:
1. **Create Excel File in OneDrive for Business:**
   - Creates a new Excel file with specified details.

2. **Generate Shareable Link:**
   - Generates a shareable link for the created Excel file.

3. **Post Message in Teams Chat:**
   - Posts a message in a Teams chat with the shareable link.

### If the current day is the 22nd (Reminder):
1. **Create Excel File in OneDrive for Business:**
   - Creates a new Excel file with specified details.

2. **Generate Shareable Link:**
   - Generates a shareable link for the created Excel file.

3. **Post Reminder Message in Teams Chat:**
   - Posts a reminder message in a Teams chat with the shareable link.

### If the current day is the 24th (Final Reminder):
1. **Create Excel File in OneDrive for Business:**
   - Creates a new Excel file with specified details.

2. **Generate Shareable Link:**
   - Generates a shareable link for the created Excel file.

3. **Post Final Reminder Message in Teams Chat:**
   - Posts a final reminder message in a Teams chat with the shareable link.

## Business Benefits:

1. **Efficiency and Automation:**
   - The Power Automate flow significantly reduces manual effort and potential human errors associated with routine tasks, enhancing overall efficiency and accuracy.

2. **Timely Communication:**
   - By automatically posting messages in Teams chats on the 15th, 22nd, and 24th of each month, the flow ensures timely communication of important updates, file creations, and reminders. This minimizes the risk of information gaps and keeps team members well-informed.

3. **Collaboration and Document Sharing:**
   - Creating Excel files in OneDrive for Business and generating shareable links streamline collaboration. Team members can effortlessly access shared files, fostering a culture of collaboration and knowledge-sharing within the organization.

4. **Task Reminders:**
   - Acting as a reminder system for important tasks or deadlines associated with the 22nd and 24th of each month, the flow helps teams stay on track. This is particularly crucial for meeting project milestones, completing reports, or handling other time-sensitive activities.

5. **Consistency and Standardization:**
   - The automation ensures that the same set of actions is performed consistently based on the day of the month. This standardization reduces variability in processes, contributing to a more organized and predictable workflow.

6. **Centralized Data Storage:**
   - Storing Excel files in OneDrive for Business promotes centralized data storage. This centralization facilitates easy access for team members, fostering an organized approach to document management.

7. **Enhanced Communication in Teams:**
   - Utilizing Teams for communication ensures that relevant information is shared in a platform familiar to team members. This integration enhances communication within the organization, creating a centralized hub for updates and collaboration.

## NOTES:
Update "manifest.json" with your offical email id.
