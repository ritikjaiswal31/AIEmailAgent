## AIMailFlow 📧

### AI Assisted Email Automation System

---

### Project Overview

AIMailFlow is an AI-powered email response system that integrates with Gmail to generate context-aware replies in real time. The application is built using **Spring Boot** on the backend, **React** on the frontend, and **Gemini AI** for intelligent email response generation. A **Chrome Extension** seamlessly injects AI-assisted reply functionality directly into the Gmail interface to streamline email communication and improve response efficiency.

---

### Real-World Use Case

* In many professional environments, employees, support teams and business professionals spend significant time drafting repetitive email responses such as meeting confirmations, client follow-ups, operational communications and support acknowledgements.

* Repeatedly writing these responses increases manual effort, slows communication workflows and reduces overall productivity.

* AIMailFlow was designed to solve this problem by integrating AI-assisted email reply generation directly into Gmail.

* Instead of switching between external AI tools and email clients, users can generate context-aware responses within their existing Gmail workflow using a single click.

* The system combines browser automation, backend orchestration and AI-powered response generation to streamline routine communication workflows.

* The Chrome Extension captures email content directly from Gmail, while the Spring Boot backend processes requests, dynamically constructs prompts and communicates with Gemini AI APIs using WebClient.

* The generated response is then returned to the Gmail interface in real time for seamless AI-assisted email drafting.

* The workflow can be applied to several real-world scenarios including customer support communication, HR response automation, client engagement workflows, sales outreach and repetitive enterprise email handling where response efficiency and productivity are critical.

---

### Key Features

* AI-powered email reply generation using **Gemini AI**
* Context-aware response generation based on email content
* Gmail-integrated Chrome Extension for one-click AI replies
* RESTful APIs for email processing and AI communication
* Real-time backend request handling using **WebClient**
* Browser-assisted workflow integration within Gmail
* API testing and validation using **Postman**

---

### Tech Stack

| Category          | Technologies         |
| ----------------- | -------------------- |
| Backend           | Java, Spring Boot    |
| Frontend          | React                |
| AI Integration    | Gemini AI, WebClient |
| Browser Extension | Chrome Extension     |
| API Testing       | Postman              |
| Communication     | REST APIs            |

---

### High-Level Design (HLD)

┌────────────────────┐
│     Gmail UI       │
│                    │
│ User opens email   │
│ Clicks AI Reply    │
└─────────┬──────────┘
          │
          ▼
┌────────────────────┐
│ Chrome Extension   │
│                    │
│ Content Script     │
│ DOM Manipulation   │
│ Toolbar Injection  │
│ Email Extraction   │
└─────────┬──────────┘
          │ HTTPS
          ▼
┌────────────────────┐
│ Spring Boot API    │
│                    │
│ Request Validation │
│ Prompt Building    │
│ Gemini Orchestration│
└─────────┬──────────┘
          │ HTTPS
          ▼
┌────────────────────┐
│ Gemini API         │
│                    │
│ Generate Reply     │
└─────────┬──────────┘
          │
          ▼
┌────────────────────┐
│ Gmail Compose Box  │
│                    │
│ Reply Inserted     │
│ User Reviews       │
│ User Sends Email   │
└────────────────────┘

---

### Low-Level Design (LLD)

<img width="1536" height="506" alt="AIMailFlow LLD" src="https://github.com/user-attachments/assets/802a188e-5569-4046-bae3-d2562990198e" />

---

### Screenshots  

Below are the key components of **AIMailFlow** shown in a logical order, starting from the **end-user experience** to the **underlying implementation**.  

#### AI Reply in Gmail

<img width="1486" height="644" alt="image" src="https://github.com/user-attachments/assets/52f18005-dee4-40be-ad52-7eaab2651571" />

<img width="1490" height="712" alt="image" src="https://github.com/user-attachments/assets/30fff2db-a3c6-4464-81c8-80865ac97426" />

---

### Chrome Extension

<img width="1009" height="626" alt="Screenshot 2025-08-29 031232" src="https://github.com/user-attachments/assets/55c94846-9299-4cc2-9616-599bdbaa8815" />

---

#### Frontend Service

<img width="1429" height="886" alt="image" src="https://github.com/user-attachments/assets/6bb40bb4-55f7-46a8-a32c-774039af2634" />

<img width="1077" height="758" alt="Screenshot 2026-01-01 034230" src="https://github.com/user-attachments/assets/27594374-0863-4c62-914e-47ed2296d195" />

<img width="1071" height="762" alt="Screenshot 2026-01-01 034251" src="https://github.com/user-attachments/assets/c5b1c7bf-3d18-407f-be14-60818e11b7c4" />

<img width="1074" height="756" alt="Screenshot 2026-01-01 034311" src="https://github.com/user-attachments/assets/4c292404-117e-4129-b85d-e37a5146c218" />

---

#### Backend Service 

<img width="1502" height="648" alt="image" src="https://github.com/user-attachments/assets/5dcfbcc3-bf2b-4114-97e9-a8431aa3ad7a" />

<img width="1377" height="591" alt="image" src="https://github.com/user-attachments/assets/c364fe2d-22d4-4737-81d0-e5761616a78d" />

---

#### Postman Testing

<img width="1417" height="657" alt="image" src="https://github.com/user-attachments/assets/0baf852f-7de6-4a6e-8a24-52b2170a3784" />

<img width="1422" height="700" alt="image" src="https://github.com/user-attachments/assets/e8c7ca45-659e-4695-833a-ed6f4998cf14" />
