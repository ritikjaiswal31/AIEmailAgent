# AIEmailAgent 📧
**Intelligent Email Reply Agent**

AIEmailAgent is an intelligent email reply system that seamlessly integrates with **Gmail**, enabling users to generate **context-aware AI responses** in real time.  
The application is built using **Spring Boot** and **Spring AI** on the backend, **React** on the frontend, and **Google Gemini AI** for natural language response generation. A **Chrome Extension** embeds AI functionality directly into the Gmail interface.

---

## Key Features

- **AI-Powered Email Reply Generation** using Google Gemini AI  
- **Context-Aware Responses** based on email content  
- **Chrome Extension Integration** with Gmail for one-click AI replies  
- **RESTful APIs** for email processing and AI communication  
- **Secure Backend Architecture** with Spring Boot  
- **API Validation & Testing** using Postman  

---

## Architecture

AIEmailAgent follows a **modular client-server architecture**:
- Chrome Extension injects an **“AI Reply” button** into the Gmail UI  
- Frontend (React) communicates with backend REST APIs  
- Backend (Spring Boot + Spring AI) handles business logic and AI orchestration  
- Google Gemini AI generates intelligent email responses  
- APIs are designed for scalability, security, and testability  

---

## Tech Stack

| Category | Technologies |
|--------|--------------|
| Frontend | React |
| Backend | Spring Boot |
| AI Integration | Spring AI, Google Gemini AI |
| API Testing | Postman |
| Browser Extension | Chrome Extension |
| Communication | REST APIs |

---

## Modules

| Module | Description |
|------|-------------|
| **Chrome Extension** | Injects the AI Reply button into Gmail |
| **frontend-app** | React-based UI for configuration and testing |
| **email-service** | Extracts and processes email content |
| **ai-service** | Integrates with Google Gemini AI via Spring AI |
| **api-layer** | Exposes REST endpoints for frontend and extension |

---

## Application Flow

1. User opens an email in **Gmail**
2. Chrome Extension injects the **AI Reply** button
3. Email content is sent to the backend via REST API
4. Backend processes the request using **Spring AI**
5. **Google Gemini AI** generates a context-aware reply
6. The AI-generated response is returned and displayed to the user

---

## Screenshots  

Below are the key components of **AIEmailAgent** shown in a logical order, starting from the **end-user experience** to the **underlying implementation**.  

### AI Reply in Gmail

<img width="1486" height="644" alt="image" src="https://github.com/user-attachments/assets/52f18005-dee4-40be-ad52-7eaab2651571" />

<img width="1490" height="712" alt="image" src="https://github.com/user-attachments/assets/30fff2db-a3c6-4464-81c8-80865ac97426" />

---

### Chrome Extension

<img width="1009" height="626" alt="Screenshot 2025-08-29 031232" src="https://github.com/user-attachments/assets/55c94846-9299-4cc2-9616-599bdbaa8815" />

---

### Frontend UI

<img width="1429" height="886" alt="image" src="https://github.com/user-attachments/assets/6bb40bb4-55f7-46a8-a32c-774039af2634" />

<img width="1077" height="758" alt="Screenshot 2026-01-01 034230" src="https://github.com/user-attachments/assets/27594374-0863-4c62-914e-47ed2296d195" />

<img width="1071" height="762" alt="Screenshot 2026-01-01 034251" src="https://github.com/user-attachments/assets/c5b1c7bf-3d18-407f-be14-60818e11b7c4" />

<img width="1074" height="756" alt="Screenshot 2026-01-01 034311" src="https://github.com/user-attachments/assets/4c292404-117e-4129-b85d-e37a5146c218" />

---

### Backend Service 

<img width="1502" height="648" alt="image" src="https://github.com/user-attachments/assets/5dcfbcc3-bf2b-4114-97e9-a8431aa3ad7a" />

<img width="1377" height="591" alt="image" src="https://github.com/user-attachments/assets/c364fe2d-22d4-4737-81d0-e5761616a78d" />

---

### Postman Testing

<img width="1417" height="657" alt="image" src="https://github.com/user-attachments/assets/0baf852f-7de6-4a6e-8a24-52b2170a3784" />

<img width="1422" height="700" alt="image" src="https://github.com/user-attachments/assets/e8c7ca45-659e-4695-833a-ed6f4998cf14" />
