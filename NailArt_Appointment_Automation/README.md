# 💅 NailArt Appointment Automation  

The **NailArt Appointment Automation System** is an AI-powered workflow built using **n8n**.  
It automates appointment scheduling by interacting with users through chat, processing their requests via an **AI Agent + Google Gemini Model**, and managing all appointments in **Google Calendar**.  

---

## 📸 System Architecture  

[NailArt Appointment Flow](./Nailartworkflow.png)  

Live demo=https://surajmaurya1.app.n8n.cloud/webhook/e3edb768-0d0f-40cb-b4d4-2cd8a51263fc/chat

WebsiteHome=(./websitehome.png)

## 🚀 Introduction  

Managing salon appointments manually can be messy and prone to errors.  
This project introduces an **automated AI scheduling assistant** that:  

1. Receives user requests via **chat messages**  
2. Uses an **AI Agent** with the **Google Gemini Chat Model** to understand intent  
3. Interacts with **Google Calendar** to create, fetch, or delete appointments  
4. Uses **memory** to track ongoing conversations  

With this system, clients can easily schedule, modify, or cancel their nail art appointments through an AI-driven automation.  

---

## ✨ Features  

- ✅ AI-driven chat-based appointment scheduling  
- ✅ Automatic creation of appointments in Google Calendar  
- ✅ Fetch all scheduled appointments instantly  
- ✅ Cancel or update existing appointments  
- ✅ Conversation memory for better user interaction  
- ✅ Fully automated salon booking workflow  

---

## 🛠️ Tech Stack  

- **Automation Platform**: n8n  
- **AI/ML Model**: Google Gemini Chat Model  
- **Database/Logs**: Google Calendar Events  
- **Communication**: Chat-based input  
- **Memory**: Simple Memory for user context  
- **Agent**: n8n AI Agent for workflow control  

---

## ⚙️ Workflow Explanation  

1. **Chat Input (n8n Tool: When Chat Message Received)**  
   - Captures user requests (e.g., "Book appointment for 3 PM tomorrow").  

2. **AI Agent (n8n Tool)**  
   - Processes the chat message and decides the next step.  
   - Works with **Gemini AI Model** for natural language understanding.  

3. **Google Gemini Chat Model**  
   - Understands user’s intent and helps AI Agent in decision-making.  

4. **Google Calendar (n8n Tools)**  
   - **Create Event** → Books a new appointment.  
   - **Get All Events** → Retrieves all scheduled appointments.  
   - **Delete Event** → Cancels an existing appointment.  

5. **Simple Memory**  
   - Stores context so users can have smooth, ongoing conversations.  

---

## 📊 Example Use Case  

A client sends:  
- *"I want to book a nail art appointment tomorrow at 4 PM."*  

➡ The system will:  
- Process the request with the AI Agent + Gemini Model  
- Create a new event in **Google Calendar** at 4 PM tomorrow  
- Save the context in memory for further follow-ups (e.g., reschedule/cancel)  

If the client later says:  
- *"Cancel my 4 PM appointment"*  
➡ The system will automatically delete that event from the calendar.  



## 🔧 Tools in n8n  

This project uses the following n8n nodes/tools:  

- **When Chat Message Received** → For capturing client requests  
- **AI Agent Node** → For processing requests and coordinating tasks  
- **Google Gemini Model Node** → For understanding user intent  
- **Google Calendar Create Event Node** → For adding new appointments  
- **Google Calendar Get All Events Node** → For viewing schedules  
- **Google Calendar Delete Event Node** → For canceling appointments  
- **Simple Memory Node** → For maintaining conversation flow  