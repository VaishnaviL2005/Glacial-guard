# 🏔️ GlacialGuard

GlacialGuard is a full-stack application designed to monitor Himalayan glaciers and glacial lakes 🏞️. It assesses risks using AI 🤖 and sends real-time alerts 📡 to communities. Built with React, TypeScript, Supabase, and a Python-based AI model, it offers tailored dashboards for admins and citizens 🧑‍💼 and supports multilingual alerts 🗣️.

## ✨ Features

*   ✅ **Real-time Glacier Monitoring:** Provides up-to-date information on the state of Himalayan glaciers.
*   🤖 **AI-Powered Risk Assessment:** Uses a Python-based AI model to predict potential risks.
*   🔑 **Role-Based Access:** Tailored dashboards for admin and citizen users.
*   💬 **Community Feedback:** Allows community members to submit reports and feedback.
*   🗣️ **Multilingual Support:** Supports alerts and information in multiple languages.

## 🛠️ Technologies Used

*   **Client:** React, TypeScript, Vite, Shadcn-UI, Tailwind CSS
*   **Server:** Node.js, Express, TypeScript
*   **Database & Authentication:** Supabase
*   **AI Model:** Python, Flask, joblib, scikit-learn

## 🚀 Client Setup

1.  Navigate to the client directory: `cd client`
2.  Install dependencies: `npm install`
3.  Create a `.env` file and add Supabase credentials (see [client/README.md](https://github.com/Naimish08/Glacial-guard/blob/main/client/README.md) for details).
4.  Start the development server: `npm run dev`

## ⚙️ Server Setup

Follow the instructions in [SERVER_SETUP.md](https://github.com/Naimish08/Glacial-guard/blob/main/SERVER_SETUP.md) to set up and run the server.

1.  Navigate to the server directory: `cd server`
2.  Install dependencies: `npm install`
3.  Start the server: `npm run dev`

## 🐍 Python Service Setup

1.  Navigate to the python-service directory: `cd python-service`
2.  Install the required Python packages: `pip install -r requirements.txt`
3.  Start the Flask application: `python app.py`

## 🔑 Role-Based Access

*   🧑‍💼 **Admin Users:** Full administrative dashboard, including the Model Input Form and advanced alert management.
*   👤 **Citizen Users:** Citizen dashboard with public information, alerts, and community sections.


## ⚙️ API Endpoints

The server exposes the following API endpoints:

*   `POST /api/community/reports` - Submit community reports
*   `GET /api/community/reports` - Get community reports
*   `POST /api/community/missing-persons` - Submit missing person reports
*   `GET /api/community/missing-persons` - Get missing person reports
*   `GET /api/uploads/:filename` - Serve uploaded images
*   `POST /api/alerts/sms` - Send SMS alerts
*   `POST /api/alerts/whatsapp` - Send Whatsapp alerts
*   `POST /api/alerts/emergency` - Send Emergency alerts using SMS and Whatsapp
*   `POST /api/alerts/multilingual-emergency` - Send emergency alerts in multiple languages based on Glacier contact details

## 🗺️ Sequence Diagram

Here's a sequence diagram illustrating how the client interacts with the server and Python service:

<img width="2922" height="2242" alt="Untitled diagram-2025-10-13-060757" src="https://github.com/user-attachments/assets/af8aaa38-d9fb-42d4-9936-4190cd422879" />
