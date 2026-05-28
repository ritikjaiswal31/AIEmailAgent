# AIMailFlow 📧

### AI-Powered Email Reply Flow

## Project Overview

AIMailFlow is an AI-powered email response system that integrates with Gmail to generate context-aware replies in real time. The application is built using **Spring Boot** on the backend, **React** on the frontend, and **Google Gemini AI** for intelligent email response generation. A **Chrome Extension** seamlessly injects AI-assisted reply functionality directly into the Gmail interface to streamline email communication and improve response efficiency.

---

# Key Features

* AI-powered email reply generation using **Google Gemini AI**
* Context-aware response generation based on email content
* Gmail-integrated Chrome Extension for one-click AI replies
* RESTful APIs for email processing and AI communication
* Real-time backend request handling using **WebClient**
* Browser-assisted workflow integration within Gmail
* API testing and validation using **Postman**

---

# Tech Stack

| Category          | Technologies                |
| ----------------- | --------------------------- |
| Backend           | Java, Spring Boot           |
| Frontend          | React                       |
| AI Integration    | Google Gemini AI, WebClient |
| Browser Extension | Chrome Extension            |
| API Testing       | Postman                     |
| Communication     | REST APIs                   |

---

# High-Level Design (HLD)

AIMailFlow follows a modular client-server architecture for seamless AI-assisted email response generation.

## Core Components

### 1. Chrome Extension

* Injects the **AI Reply** button into the Gmail compose interface
* Captures email content directly from Gmail
* Sends requests to backend APIs

### 2. Frontend Application

* React-based interface for testing and configuration
* Allows users to generate AI replies outside Gmail workflows

### 3. Backend Service

* Built using Spring Boot REST APIs
* Handles request processing, prompt generation and AI orchestration
* Communicates with Gemini AI APIs using WebClient

### 4. Gemini AI

* Generates context-aware email replies
* Supports dynamic response generation based on email tone and content

---

# Low-Level Design (LLD)

## Backend Modules

| Module                     | Responsibility                                                  |
| -------------------------- | --------------------------------------------------------------- |
| `EmailGeneratorController` | Exposes REST endpoints for email reply generation               |
| `EmailGeneratorService`    | Handles prompt creation, API communication and response parsing |
| `EmailRequest`             | DTO for email content and tone handling                         |
| `WebClient`                | Sends asynchronous HTTP requests to Gemini AI APIs              |
| `ObjectMapper`             | Parses AI-generated JSON responses                              |

---

# Architecture Flow

```text id="3k9p2x"
User Opens Gmail
        ↓
Chrome Extension Injects "AI Reply" Button
        ↓
Email Content Extracted From Gmail
        ↓
REST API Request Sent To Spring Boot Backend
        ↓
Backend Builds Prompt & Sends Request Using WebClient
        ↓
Google Gemini AI Generates Context-Aware Reply
        ↓
Backend Processes AI Response
        ↓
Generated Reply Returned To Gmail UI
```

---

# Application Flow

1. User opens an email in Gmail
2. Chrome Extension injects the AI Reply button
3. Email content is extracted from Gmail UI
4. Backend receives the email content via REST API
5. Prompt is dynamically generated based on email tone and content
6. WebClient sends request to Gemini AI API
7. AI-generated response is parsed and processed
8. Final response is displayed inside Gmail for one-click usage

---

# Conclusion

AIMailFlow demonstrates the integration of AI-powered workflows with real-world browser automation and backend API orchestration. The project combines Spring Boot, REST APIs, Chrome Extension development and Gemini AI integration to deliver seamless AI-assisted email reply generation directly within Gmail.

---

## Screenshots  

Below are the key components of **AIMailFlow** shown in a logical order, starting from the **end-user experience** to the **underlying implementation**.  

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
