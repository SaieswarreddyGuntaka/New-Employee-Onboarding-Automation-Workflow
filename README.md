# New Employee Onboarding Automation Workflow

This project automates the new employee onboarding process using Microsoft Power Automate and Microsoft 365 tools. It ensures a smooth, consistent, and error-free experience for every new hire.

---

## 🌟 Goal

Automate repetitive onboarding tasks so that HR, IT, and managers can focus on the human aspects of onboarding.

---

## ✅ Features

- Auto-create user accounts in Azure AD
- Assign licenses (e.g., M365)
- Notify IT for hardware setup
- Schedule orientation meetings
- Share onboarding documents
- Generate 30/60/90 day task checklist
- Post notifications in Teams
- Track onboarding progress in SharePoint

---

## 🛠 Tools Used

- **Power Automate**
- **Microsoft Forms / Power Apps**
- **Azure Active Directory**
- **Microsoft 365 / Outlook / Teams**
- **SharePoint Online**

---

## 🔁 Workflow Overview

### 🎯 Trigger
New hire form submitted via Microsoft Forms or Power Apps.

### 🧩 Automation Steps

1. **Create User in Azure AD**  
   - Uses Power Automate Azure AD connector

2. **Send Welcome Email**  
   - With links to policy docs, training, etc.

3. **Assign Licenses**  
   - Automatically assign required Microsoft 365 licenses

4. **Notify Teams**  
   - Notify IT, HR, and the team via Teams channel

5. **Schedule Orientation**  
   - Calendar invite sent for training sessions

6. **Document Sharing**  
   - Share access to employee handbook, onboarding portal, and policies

7. **Update SharePoint Tracker**  
   - Add user info to central onboarding tracker

---

## 📁 Files Included

- `workflow_diagram.png`: Visual representation of the workflow
- `sample_form_response.json`: Sample form submission data
- `welcome_email_template.html`: Template for welcome email
- `onboarding_tasks_checklist.xlsx`: Sample 30/60/90 day checklist

---

## 🤝 Contributions

Pull requests are welcome! Feel free to enhance the automation or add support for other systems like Google Workspace, Slack, etc.

---

## 📄 License

MIT License


---

## ⚙️ Power Automate Flow

The core automation logic is stored in `power_automate_flow.json`, a JSON file you can import into Power Automate:

**Steps to Use It**:
1. Go to [Power Automate](https://flow.microsoft.com/).
2. Select **Import** > **Import Package (.zip)** (rename `.json` to `.zip` if needed).
3. Map the connections (Azure AD, Office 365, Teams).
4. Customize the flow with real Team/Channel IDs and additional actions if needed.

This flow handles:
- Azure AD user creation
- Sending a welcome email
- Notifying the team in Microsoft Teams

