# 🚀 AI Research Assistant (Spring Boot + Gemini API)

An AI-powered backend application that processes user input and leverages the Gemini API to generate intelligent summaries and topic suggestions.

---

## 📌 Overview

This project demonstrates real-world integration of a **Spring Boot backend** with an external **AI API (Gemini)**.

It allows users to:
- Summarize large text content
- Get intelligent topic suggestions

---

## ✨ Key Features

- 🔍 Intelligent text summarization  
- 💡 Context-based topic suggestions  
- 🌐 REST API architecture
- ✨ Lombok 
- ⚡ External API integration (Gemini)  
- 📦 JSON request/response handling  

---

## 🛠️ Tech Stack

- **Java 21**
- **Spring Boot**
- **Spring WebFlux (WebClient)**
- **Jackson (ObjectMapper)**
- **REST APIs**

---

## 🧠 System Flow

Client Request  
↓  
Controller Layer  
↓  
Service Layer (Business Logic)  
↓  
Prompt Builder  
↓  
Gemini API (External Call)  
↓  
JSON Response  
↓  
Response Parsing (ObjectMapper)  
↓  
Final Output  

---


### 🔹 Request Body
```json
{
  "operation": "summarize",
  "content": "Your text here..."
}

## 🔑 Configuration

Add your Gemini API credentials in application.properties:

gemini.api.url=YOUR_API_URL
gemini.api.key=YOUR_API_KEY

## 🧪 How to Run
git clone https://github.com/mrdinesh-kushwaha/AI-Research-Assistant.git
cd AI-Research-Assistant
mvn spring-boot:run
