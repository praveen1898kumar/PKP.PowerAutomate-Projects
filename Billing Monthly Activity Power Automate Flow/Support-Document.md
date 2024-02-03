# Flow Documentation for Billing Activity:

## Flow 1: Billing Validation and Notification

**Trigger:** Daily at 10 AM (India Standard Time)

1. **Condition Check:**
   - Checks if the current day of the month is the 18th.

2. **File Copy:**
   - Copies a file from a template folder to a billing sheet folder.

3. **Share Link Creation:**
   - Creates a share link for editing the copied file.

4. **Data Retrieval:**
   - Retrieves rows from a table in the file.

5. **Filtering:**
   - Filters rows with a total billable hours value of 0.

6. **Onsite Members Email Notification:**
   - Retrieves rows for onsite members from the same table.
   - Sends an email to onsite members with a predefined message if zero billable hours are found.

7. **Teams Chat Notification:**
   - Posts a message in a Teams chat with a URL to the shared file.

**Benefits:**
- Automated daily checks ensure timely billing activities.
- Identifies instances of zero billable hours for immediate attention.
- Streamlines communication with onsite members through automated emails.
- Enhances collaboration by sharing billing information in Teams.

---

## Flow 2: Monthly Billing Sheet Creation and Non-submission Alerts

**Trigger:** Daily at 10 AM (India Standard Time)

1. **File Copy:**
   - Copies a template billing sheet to a new file with the current month and year in the file name.

2. **Data Retrieval:**
   - Retrieves rows from a table in the billing sheet.

3. **Filtering:**
   - Identifies members who have not filled in their billable hours for the current month.

4. **Notification Preparation:**
   - Collects names and email addresses of members with missing billable hours.

5. **Email Notification:**
   - Sends an email to identified members, prompting them to fill in their billable hours.

6. **Teams Chat Notification:**
   - Posts a message in a chat to remind members to update their billable hours.

**Benefits:**
- Ensures the creation of monthly billing sheets with current data.
- Proactively identifies members with missing billable hours.
- Streamlines communication through automated email reminders and Teams messages.

---

## Flow 3: Billing Reminder on the 21st of the Month

**Trigger:** Daily at 10 AM (India Standard Time) if the current day is the 21st

1. **Condition Check:**
   - Verifies if the current day of the month is the 21st.

2. **File Copy:**
   - Copies a billing sheet template to a new file with the current month and year in the file name.

3. **Data Retrieval:**
   - Retrieves rows from a table in the billing sheet.

4. **Filtering:**
   - Identifies members who have not filled in their billable hours for the current month.

5. **Reminder Actions:**
   - Sends an email reminder to members with missing billable hours.
   - Posts a message in a Teams chat to prompt members to update their billable hours.

**Benefits:**
- Specific reminder on the 21st ensures attention to billing completeness.
- Reinforces communication through both email and Teams messages.
- Encourages timely updates from team members.
