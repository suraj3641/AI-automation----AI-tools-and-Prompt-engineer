# 🌍 AI Travel Planner  

AI Travel Planner is an intelligent automation-based project that generates personalized travel itineraries based on user preferences such as budget, location, facilities, and area etc.  
The workflow is built using **n8n** and tools like **Webhook → AI Agent → Google Gemini Model → Google Sheets → Gmail**.  

---

## System Architecture  

[AI Travel Planner Flow](./Workflow.png)  


## 🚀 Introduction  

This project is designed to make traveling smarter and more efficient.  
Users provide their input (name, email, budget, location, facilities, etc.), which is collected via a webhook.  
The **AI Agent** processes the data and interacts with the **Google Gemini Model** to generate an intelligent itinerary.  

The generated plan is automatically saved in **Google Sheets** for tracking and also sent to the user instantly via **Gmail**.  

---

## ✨ Features  

- ✅ User-friendly input form (Name, Email, Location, Budget, etc.)  
- ✅ AI-driven personalized travel plan generation  
- ✅ Automatic data logging into Google Sheets  
- ✅ Instant delivery of the plan via Gmail  
- ✅ Scalable & fully automated workflow using n8n  

---

## 🛠️ Tech Stack  

- **Automation Platform**: n8n  
- **AI/ML Model**: Google Gemini Chat Model  
- **Database/Logs**: Google Sheets  
- **Communication**: Gmail  
- **Webhook**: Input data collection  
- **Agent**: n8n AI Agent for workflow intelligence  

---

##  Workflow Explanation  

1. **Webhook (n8n Tool)**  
   - Captures user inputs such as name, email, budget, location, and facilities.  

2. **AI Agent (n8n Tool)**  
   - Acts as the central processing unit.  
   - Connects the webhook data to the Google Gemini Chat Model.  
   - Handles logic, memory, and tool integrations.  

3. **Google Gemini Chat Model**  
   - Processes the inputs and generates a personalized travel itinerary.  

4. **Google Sheets (n8n Tool)**  
   - Appends or updates a row in the sheet for every request.  
   - Helps maintain records of all itineraries generated.  

5. **Gmail (n8n Tool)**  
   - Sends the generated itinerary instantly to the user’s email.  

---

## 📊 Example Use Case  

A user enters:  
- Name: Suraj  
- Location: Goa  
- Budget: ₹25,000  
- Facilities: Beach View Hotel, Adventure Sports  

➡ The system generates a **4–5 day itinerary**, sends it to the user’s Gmail, and logs the request in Google Sheets.  

---

## 🔧 Tools in n8n  

This project uses the following n8n nodes/tools:  

- **Webhook Node** → For receiving user inputs  
- **AI Agent Node** → For processing inputs and integrating with AI models  
- **Google Gemini Model Node** → For generating personalized itineraries  
- **Google Sheets Node** → For storing logs and user data  
- **Gmail Node** → For sending the travel plan via email  
