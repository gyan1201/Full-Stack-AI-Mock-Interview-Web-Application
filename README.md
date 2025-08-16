# Full-Stack-AI-Mock-Interview-Web-Application
Built an AI-powered full-stack web app for mock interviews, featuring live AI avatar interviews, automated real-time feedback, and secure subscription management.

# 🤖 Full-Stack AI Mock Interview Platform  

An end-to-end **AI-powered SaaS application** built from scratch to help users **prepare for job interviews** with realistic **AI-driven mock interview sessions**.  

The platform features a **live streaming AI avatar interviewer**, **real-time feedback**, and a **subscription model**, combining the power of AI with modern full-stack development practices.  

---

## 🚀 Key Features  

### 🎯 AI-Driven Interview Generation  
- Generates interview questions based on **uploaded resumes (PDF)** or **job descriptions**.  
- Automated workflows powered by **n8n** for drag-and-drop orchestration.  
- **ImageKit** integration for free cloud storage and resume text extraction.  
- **OpenAI / Gemini** models generate tailored interview questions + analyze conversations.  

### 🗣️ Interactive Interview Experience  
- **Akool Streaming Avatar API** conducts **live interviews** with real-time interaction.  
- Displays **conversation transcripts** during sessions.  
- In-call controls: **mute/unmute** and **end call**.  

### 📊 Automated Feedback & Reporting  
- Generates **detailed feedback** (strengths, suggestions, rating out of 10).  
- Uses **n8n AI workflows** to process interview conversations.  
- Feedback stored in user dashboard for review anytime.  

### 🔐 User Management & Security  
- **Clerk** for secure authentication (Gmail, email/password, social login).  
- Subscription billing with free & paid tiers (limit free users to 2 interviews/day).  
- **Arja** for rate limiting, bot detection, email validation, and attack prevention.  

### 💾 Scalable Data Infrastructure  
- **Convex DB** (real-time, open-source) for storing sessions, users, and app data.  
- Designed schemas for **user profiles & interview sessions** with relationships.  

### 💻 Modern Web Development Stack  
- **React + Next.js** (folder-based routing, RSC, client/server rendering).  
- **Tailwind CSS** + **ShadCN** + **Aceternity UI** for sleek UI.  
- **React Context API** for global state management.  
- **TypeScript** for type safety and code quality.  

### ☁️ Deployment & Production Readiness  
- Deployed frontend to **Vercel** with CI/CD.  
- **n8n workflows** deployed on **Hostinger** for scalable AI automation.  

---

## 🛠️ Tech Stack  

- **Frontend**: React, Next.js, Tailwind CSS, ShadCN, Aceternity UI  
- **Backend/Automation**: n8n, OpenAI/Gemini, Convex DB  
- **Auth & Billing**: Clerk (OAuth, MFA, Stripe billing)  
- **AI Avatar**: Akool API (live streaming interviews)  
- **Storage**: ImageKit (resume storage & parsing)  
- **Security**: Arja (rate limiting, bot detection)  
- **Deployment**: Vercel (frontend), Hostinger (n8n workflows)  

---

## 📷 Screenshots  


