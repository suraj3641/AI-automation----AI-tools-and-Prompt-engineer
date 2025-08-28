# 🤖 Telegram Voice-to-Voice AI Chatbot  

This project is a **Telegram chatbot** that allows users to send **voice messages**, which are then:  

1. **Transcribed** into text  
2. **Processed by Google Gemini AI** for intelligent responses  
3. **Converted back into speech**  
4. Sent as a **reply audio message** on Telegram  

Built with **n8n workflow automation** + **Google Gemini AI**.  

---

## 📸 Workflow Screenshot  

[Telegram Voice Bot Workflow](./workflow.png)  

[Telegrambot](./telegrambot.png)


## 🚀 Features  

- 🎤 Accepts **voice messages** from Telegram  
- ✍️ Transcribes audio (ElevenLabs)→ text automatically  
- 🧠 Uses **Google Gemini AI** for contextual replies  
- 🔊 Converts AI responses back into **voice/audio**(ElevenLabs)  
- 📩 Sends AI voice reply directly to the Telegram user  
- 🔄 Fully automated workflow in **n8n**  

---

## ⚙️ Workflow Explanation  

1. **Telegram Trigger**  
   - Detects incoming messages (voice).  

2. **Get File**  
   - Downloads the audio message from Telegram.  

3. **Transcribe Audio or Video(ElevenLabs)**  
   - Converts speech into text.  

4. **AI Agent (Google Gemini Chat Model)**  
   - Processes the transcribed text and generates an intelligent response.  

5. **Convert Text to Speech(ElevenLabs)**  
   - Converts Gemini’s text reply back into audio.  

6. **Send Audio File**  
   - Sends the generated voice reply to the user on Telegram.  

---

## 🛠️ Tech Stack  

- **n8n** (workflow automation)  
- **Telegram Bot API**  
- **Google Gemini AI** (chat model)  
- **Speech-to-Text API** (transcription)  
- **Text-to-Speech API** (reply audio generation)  



## 📊 Example Use Case  

👤 User sends: 🎤 *“What is the weather today in Delhi?”*  

➡ Workflow:  
1. Telegram bot receives audio  
2. Transcribes speech(ElevenLabs) → "What is the weather today in Delhi?"  
3. Gemini AI generates response → "Today in Delhi, the weather is sunny with a high of 35°C."  
4. Converts text(ElevenLabs) → speech  
5. Sends back a **voice reply** to the user  
