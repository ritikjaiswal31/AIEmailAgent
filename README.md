# AIMailFlow 📧

### AI-Powered Email Reply Flow

---

## Project Overview

AIMailFlow is an AI-powered email response system that integrates with Gmail to generate context-aware replies in real time. The application is built using **Spring Boot** on the backend, **React** on the frontend, and **Gemini AI** for intelligent email response generation. A **Chrome Extension** seamlessly injects AI-assisted reply functionality directly into the Gmail interface to streamline email communication and improve response efficiency.

---

## Real-World Use Case

* In many professional environments, employees, support teams and business professionals spend significant time drafting repetitive email responses such as meeting confirmations, client follow-ups, operational communications and support acknowledgements.

* Repeatedly writing these responses increases manual effort, slows communication workflows and reduces overall productivity.

* AIMailFlow was designed to solve this problem by integrating AI-assisted email reply generation directly into Gmail.

* Instead of switching between external AI tools and email clients, users can generate context-aware responses within their existing Gmail workflow using a single click.

* The system combines browser automation, backend orchestration and AI-powered response generation to streamline routine communication workflows.

* The Chrome Extension captures email content directly from Gmail, while the Spring Boot backend processes requests, dynamically constructs prompts and communicates with Gemini AI APIs using WebClient.

* The generated response is then returned to the Gmail interface in real time for seamless AI-assisted email drafting.

* The workflow can be applied to several real-world scenarios including customer support communication, HR response automation, client engagement workflows, sales outreach and repetitive enterprise email handling where response efficiency and productivity are critical.

---

## Key Features

* AI-powered email reply generation using **Gemini AI**
* Context-aware response generation based on email content
* Gmail-integrated Chrome Extension for one-click AI replies
* RESTful APIs for email processing and AI communication
* Real-time backend request handling using **WebClient**
* Browser-assisted workflow integration within Gmail
* API testing and validation using **Postman**

---

## Tech Stack

| Category          | Technologies         |
| ----------------- | -------------------- |
| Backend           | Java, Spring Boot    |
| Frontend          | React                |
| AI Integration    | Gemini AI, WebClient |
| Browser Extension | Chrome Extension     |
| API Testing       | Postman              |
| Communication     | REST APIs            |

---

## High-Level Design (HLD)

AIMailFlow follows a modular client-server architecture for seamless AI-assisted email response generation.

### Core Components

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

## Low-Level Design (LLD)

AIMailFlow follows a layered backend design for handling email processing and AI request orchestration.

### Internal Backend Components

1. `EmailGeneratorController`

   * Receives email content requests from frontend and Chrome Extension
   * Exposes REST endpoints for AI reply generation

2. `EmailGeneratorService`

   * Builds dynamic prompts using email content and tone
   * Handles Gemini AI API communication using WebClient
   * Processes and parses AI-generated responses

3. `EmailRequest`

   * DTO used for transferring email content and tone data

4. `WebClient`

   * Sends asynchronous HTTP requests to Gemini AI APIs

5. `ObjectMapper`

   * Extracts and parses generated response content from JSON payloads

---

## Backend Engineering & AI Integration

AIMailFlow implements a backend-driven AI orchestration workflow using Spring Boot and WebClient for real-time communication with Gemini AI APIs. The backend is responsible for processing email content, dynamically generating prompts, handling asynchronous API communication, parsing nested JSON responses and returning context-aware email replies to the frontend and Chrome Extension.

Instead of relying on higher-level AI abstraction frameworks, the project manually manages request payload construction, response extraction and API orchestration logic, providing deeper control over backend processing and external AI service integration. The system also supports scalable REST-based communication between Gmail-integrated browser workflows, frontend components and backend services for seamless real-time AI-assisted email generation.

---

## Architecture Flow

```text
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
Gemini AI Generates Context-Aware Reply
        ↓
Backend Processes AI Response
        ↓
Generated Reply Returned To Gmail UI
```

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
