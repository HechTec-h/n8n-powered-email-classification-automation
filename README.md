# AI-Powered Email Classification & Automation

An AI-powered email classification and automated Gmail labeling workflow built with **n8n, Google Gemini API Key, and Gmail**.

This project automatically analyzes incoming emails, identifies their purpose using AI, and assigns the appropriate Gmail label based on the email content.

## Project Overview

Managing a busy inbox can be time-consuming. This automation uses Google Gemini AI to classify incoming emails into predefined categories and automatically organizes them using Gmail labels.

The workflow runs through n8n and requires your own Gmail and Google Gemini credentials.

# Project Screenshots

This folder contains screenshots of the AI-Powered Email Classification & Automation workflow built using n8n, Google Gemini, and Gmail.

These screenshots demonstrate the workflow architecture, Gmail labels, and AI-powered email classification results.

## 1. Workflow Overview

This screenshot shows the complete n8n workflow, including the Gmail Trigger, AI Agent, Google Gemini Chat Model, Structured Output Parser, IF conditions, and Gmail labeling nodes.

<img width="440" height="367" alt="Image" src="https://github.com/user-attachments/assets/c32381ca-6635-41ca-8b1c-2e7dba5dfd6e" />

## 2. Gmail Labels

This screenshot demonstrates the Gmail labels created for organizing emails into different categories.

<img width="237" height="189" alt="Image" src="https://github.com/user-attachments/assets/17570f83-2c95-45ff-b3b0-fb52c790a123" />

## 3. n8n execution

This screenshot demonstrates that how n8n executes workflow after tiggering.

<img width="400" height="310" alt="Image" src="https://github.com/user-attachments/assets/1968479b-e65b-4bbb-b8c6-abb8738626c2" />

## 4. AI Classification Results

This screenshot shows examples of AI-powered email classification and the resulting email categories.

<img width="1183" height="547" alt="Image" src="https://github.com/user-attachments/assets/05ba3b69-824e-4f47-92e8-3c7d9a991c39" />

---

All screenshots are provided for demonstration and documentation purposes.


## Features

- Automatically detects incoming Gmail messages.
- Uses Google Gemini AI for email classification.
- Classifies emails into five predefined categories.
- Automatically applies the corresponding Gmail label.
- Supports custom Gmail and Gemini credentials.
- Built with n8n for easy customization.

## Email Categories

| Category | Description |
|---|---|
| Business | Business discussions, partnerships, collaborations, and company updates. |
| Sales & Leads | Customer inquiries, pricing requests, product inquiries, and potential sales opportunities. |
| Marketing | Promotions, newsletters, advertisements, and product announcements. |
| Legal & Compliance | Contracts, legal notices, agreements, and compliance-related emails. |
| Miscellaneous | Personal, spam, unrelated, and other emails that do not fit the above categories. |

## How It Works

1. **Gmail Trigger:** Monitors your Gmail inbox for incoming emails.
2. **AI Agent:** Sends email content to Google Gemini for analysis.
3. **Structured Output Parser:** Organizes the AI response into structured data.
4. **IF Conditions:** Checks the assigned email category.
5. **Gmail Nodes:** Applies the corresponding Gmail label automatically.

## Workflow Architecture

Gmail Trigger → AI Agent → Google Gemini → Structured Output Parser → IF Conditions → Gmail Labels

## Technologies Used

- [n8n](https://n8n.io/)
- [Google Gemini](https://ai.google.dev/)
- [Gmail](https://mail.google.com/)
- AI Agent
- Structured Output Parser
- Gmail API / OAuth2

## Installation & Setup

Follow these steps to import and configure the workflow.

### Step 1: Download the Workflow

1. Open the `workflow` folder in this repository.
2. Open `email-classification.json`.
3. Download the JSON file to your computer.

### Step 2: Import into n8n

1. Open your n8n instance.
2. Create a new workflow or open the workflow editor.
3. Open the workflow menu.
4. Select **Import from File**.
5. Choose the downloaded `email-classification.json` file.

Your workflow will now appear in the n8n editor.

### Step 3: Configure Gmail Credentials

1. Open the Gmail Trigger node.
2. Create or select your own Gmail OAuth2 credentials.
3. Connect your Gmail account.
4. Open the Gmail label nodes and assign the same Gmail credentials.

**Important:** You must configure your own Gmail account. The credentials used by the original workflow are not included.

### Step 4: Configure Google Gemini API

1. Open the Google Gemini Chat Model node.
2. Create or select your own Google Gemini API credentials.
3. Add your Gemini API key.
4. Save the credentials and select them in the node.

You can obtain a Gemini API key from [Google AI Studio](https://aistudio.google.com/).

### Step 5: Create Gmail Labels

Create these five labels in your Gmail account:

- Business
- Sales & Leads
- Marketing
- Legal & Compliance
- Miscellaneous

Open each Gmail labeling node in n8n and select the corresponding label or update its Label ID to match your Gmail account.

**Note:** Gmail label IDs are account-specific. You must configure your own label IDs after importing the workflow.

### Step 6: Test the Workflow

1. Save your workflow.
2. Test the Gmail Trigger.
3. Send test emails representing different categories.
4. Check whether Gemini classifies them correctly.
5. Verify that the corresponding Gmail labels are applied.

Once everything works correctly, activate the workflow.


## Important Notes

- This workflow requires your own Gmail and Google Gemini credentials.
- Gmail label IDs must be configured for your account.
- Review the imported workflow and test all five category conditions before activation.
- AI classification may occasionally require manual review.
- The workflow JSON does not contain ready-to-use personal credentials.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Author

**Hassan Aziz**

If you find this project useful, consider giving the repository a ⭐ on GitHub!
