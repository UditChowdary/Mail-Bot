# Mailbot – Full Stack Email Summarization Assistant

Mailbot is a full-stack AI-powered email assistant that connects securely to Gmail using Google OAuth, fetches user emails, processes them with AI summarization models, and presents a clean frontend interface for reading summaries, insights, and daily digests.

Built with a React + Vite frontend and a FastAPI backend, Mailbot aims to reduce inbox overload and help users consume email content faster.

---

## 🚀 Features

**✅ Frontend**

  - Modern UI built with React + Vite

  - Clean dashboard for viewing:

  - Email summaries

  - Digest reports

  - Categories & insights

  - Google OAuth login flow

  - API integration with backend

  - Responsive, minimal design

---

**🛠️ Backend**

  - FastAPI REST API

  - Google OAuth2 authentication

  - Gmail email fetching

  - AI-powered summarization

  - Daily digest generator

  - Notification sending via Resend

  - Secure user management

  - Automated task scheduling

  - Full Pytest test suite

---

## 🧩 Tech Stack

### Frontend:

     - React (Vite)

     - Axios

     - React Router

     - TailwindCSS

     - Context API / LocalStorage

### Backend:

     - Python 3.x

     - FastAPI

     - Google OAuth2

     - Resend Email API

     - OpenAI / LLM AI Summarization

     - Pytest

     - Uvicorn

---

## 📁 Project Structure

<img width="401" height="482" alt="image" src="https://github.com/user-attachments/assets/6684651a-0f1d-4013-b60d-a70fd53125f1" />

---

## ⚙️ Installation & Setup

🖥️ 1. Clone Repository

       git clone https://github.com/your-repo/mailbot.git
       
       cd mailbot


**🌐 Frontend Setup (React + Vite)**

1. Install dependencies

        cd frontend

        npm install
   

3. Create .env file

Include:

       VITE_BACKEND_URL=http://localhost:8000
       
       VITE_GOOGLE_CLIENT_ID=your_google_client_id


3. Run the frontend

       npm run dev

The app will be available at:

👉 http://localhost:5173

**🔧 Backend Setup (FastAPI)**

1. Create a virtual environment

        cd backend

        python -m venv venv
 
        source venv/bin/activate       # Mac/Linux

        venv\Scripts\activate          # Windows

3. Install dependencies

        pip install -r requirements.txt

4. Create a .env file

       GOOGLE_CLIENT_ID=your_client_id

       GOOGLE/_CLIENT_SECRET=your_client_secret

       RESEND_API_KEY=your_resend_api_key

       OPENAI_API_KEY=your_api_key

5. Run the backend

       uvicorn main:app --reload


The backend runs at:

👉 http://localhost:8000

---

## 🔗 Connecting Frontend & Backend

The frontend uses:

       VITE_BACKEND_URL=http://localhost:8000


The backend exposes the following key endpoints:

**📡 Backend API Endpoints**

**Auth** -

       GET /auth/google – start OAuth flow

       GET /auth/google/callback – OAuth redirect

**Emails** -

       POST /api/emails/fetch – fetch & process emails

       POST /api/emails/summarize – generate AI summaries

**Digest** -

       POST /api/digest – generate/send daily digest

**Notifications** -

       POST /api/notifications – resend notifications

**Users** -

       GET/POST /api/users – user management

---

## 🧪 Testing

### Run backend tests:

        cd backend

        ./run_tests.sh


### Includes:

   - Unit tests

   - Integration tests

   - Mocked Gmail/Resend tests

---

## 🚀 Deployment

You can deploy using:

**Frontend** - 

    - Vercel

    - Netlify

    - AWS Amplify

**Backend** -

    - Render

    - Railway

    - Fly.io

    - Heroku (Procfile included)

Ensure environment variables match production credentials.

---

## 📬 Daily Digest Workflow

    - Backend fetches emails

    - AI processes summaries

    - Digest is generated

    - Resend sends the digest via email

    - Frontend displays digest on dashboard

---

## 🙌 Contributors

Udit Chowdary – Full-stack development, backend architecture, OAuth integration
