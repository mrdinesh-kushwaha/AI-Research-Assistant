#AI Research Assistant (Spring Boot + Gemini API)
🚀 Overview

An AI-powered backend application that processes user-provided content and leverages the Gemini API to generate intelligent summaries and topic suggestions.

This project demonstrates real-world integration of Spring Boot microservice architecture with external AI APIs.

✨ Key Features
🔍 Intelligent text summarization
💡 Context-based topic suggestions
🌐 REST API architecture
⚡ External API integration (Gemini)
📦 Structured JSON request/response handling
🛠️ Tech Stack
Java 21
Spring Boot
Spring WebFlux (WebClient)
Jackson (ObjectMapper)
REST APIs
🧠 System Design / Flow
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
Final Output to Client
⚙️ API Usage
🔹 Endpoint
POST /research
🔹 Request Body
{
  "operation": "summarize",
  "content": "Your text here..."
}
🔹 Supported Operations
summarize → Generate concise summary
suggest → Suggest related topics
🔹 Response
"Generated AI response..."
🔑 Configuration

Add your API credentials:

gemini.api.url=YOUR_API_URL
gemini.api.key=YOUR_API_KEY
🧪 How to Run
git clone https://github.com/mrdinesh-kushwaha/AI-Research-Assistant.git
cd AI-Research-Assistant
mvn spring-boot:run
💡 Key Learnings
Integration of external AI APIs in backend systems
Handling structured JSON responses using Jackson
Using WebClient for non-blocking HTTP calls
Designing clean service-layer architecture
🔮 Future Enhancements
Add JWT-based authentication
Convert to fully reactive (non-blocking flow)
Add frontend (React UI)
Add caching for repeated queries
👨‍💻 Author

Dinesh Kushwaha
Software Developer | Java Backend Enthusiast
