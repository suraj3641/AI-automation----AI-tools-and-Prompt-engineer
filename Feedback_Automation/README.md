# 📝Customer Feedback Automation Form  

The **Customer Feedback Automation Form** is an automation-based project built with **n8n** that collects user feedback, processes it with an **AI Agent + Google Gemini Model**, logs it into **Google Sheets**, and sends an automated acknowledgment email via **Gmail**.  

This ensures smooth, AI-powered, and fully automated feedback handling.  

---

## System Architecture  

[Feedback Automation Flow](./feedbackworkflow.png)  

Live demo=https://preview--friends-cafe-welcome.lovable.app/

##  Introduction  

Handling feedback manually can be time-consuming and inconsistent.  
This project automates the entire process:  

1. **Webhook** collects user feedback (e.g., name, email, comments).  
2. **AI Agent** processes the feedback using the **Google Gemini Model**.  
3. **Google Sheets** stores the feedback for tracking and analytics.  
4. **Gmail** sends an automated acknowledgment message back to the user.  

This creates a seamless loop of **feedback collection → intelligent processing → storage → user acknowledgment**.  


## ✨ Features  

- ✅ Automated feedback collection through webhook  
- ✅ AI-powered processing of feedback using Gemini Model  
- ✅ Automatic logging into Google Sheets for record-keeping  
- ✅ Instant acknowledgment emails to users via Gmail  
- ✅ Scalable workflow, easy to extend with more integrations  

---

## 🛠️ Tech Stack  

- **Automation Platform**: n8n  
- **AI/ML Model**: Google Gemini Chat Model  
- **Database/Logs**: Google Sheets  
- **Communication**: Gmail  
- **Webhook**: Input collection endpoint  
- **Agent**: n8n AI Agent for workflow intelligence  

---

##  Workflow Explanation  

1. **Webhook (n8n Tool)**  
   - Captures feedback submitted by the user.  

2. **AI Agent (n8n Tool)**  
   - Central processing hub.  
   - Connects feedback data with the Gemini AI Model.  

3. **Google Gemini Chat Model**  
   - Analyzes or processes the feedback content intelligently.  

4. **Google Sheets (n8n Tool)**  
   - Stores user feedback for reporting and future analysis.  

5. **Gmail (n8n Tool)**  
   - Sends automated acknowledgment or response back to the user.  


## 📊 Example Use Case  

A user submits feedback:  
- Name: Suraj  
- Email: suraj@example.com  
- Feedback: *"The app is very helpful, but I would love to see hotel booking integration."*  

➡ The system will:  
- Log this feedback into Google Sheets.  
- Process it via AI for categorization/insights.  
- Send a thank-you email automatically to Suraj.  

---

## 🔧 Tools in n8n  

This project uses the following n8n nodes/tools:  

- **Webhook Node** → For receiving feedback inputs  
- **AI Agent Node** → For processing inputs and connecting to AI models  
- **Google Gemini Model Node** → For intelligent analysis of feedback  
- **Google Sheets Node** → For storing feedback logs  
- **Gmail Node** → For sending acknowledgment/response emails  
