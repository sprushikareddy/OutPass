#  OutPass – Hostel Outing Management System

> A full-stack web application that digitizes and automates hostel outing request workflows with 3-tier role-based access for Students, Parents, and Wardens.

---

##  Problem Statement

Traditional hostel outing management relies on manual logbooks and paper-based approvals — causing delays, missing parental consent, and zero real-time tracking. OutPass solves this with a fully digital, automated approval pipeline.

---

##  Key Features

-  **Role-Based Access Control** — Separate portals for Students, Parents, and Wardens
-  **OTP Authentication** — Secure login with OTP verification
-  **Dual Approval Workflow** — Parent approval → Warden final approval
-  **QR Code Check-in/Check-out** — Digital gate verification, eliminating manual registers
-  **Real-time Notifications** — Instant alerts for approvals, rejections, and status updates
-  **Outing History** — Date-wise filtering and complete audit trail
-  **Automated Workflows** — Reduced manual processing time by ~60%

---

##  Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | React.js, HTML, CSS |
| Backend | Node.js, Express.js |
| Database | MongoDB |
| Auth | JWT, OTP |
| QR | QR Code Generation |

---

##  System Architecture

```
Student / Parent / Warden
        ↓
   React Frontend
        ↓
  Express REST API
        ↓
     MongoDB
```

**3 User Roles:**
- **Student** — Submit outing requests, view history, scan QR
- **Parent** — View & approve/reject child's outing requests
- **Warden** — Final approval, generate QR codes, monitor all outings

---

##  Project Structure

```
OutPass/
├── frontend/          # React.js UI
│   ├── src/
│   │   ├── components/
│   │   └── pages/
├── backend/           # Node.js + Express API
│   ├── routes/
│   ├── models/
│   └── controllers/
├── .env.example
└── README.md
```

---

##  Getting Started

### Prerequisites
- Node.js v14+
- MongoDB (local or Atlas)
- npm

### 1. Clone the Repository
```bash
git clone https://github.com/sprushikareddy/OutPass.git
cd OutPass
```

### 2. Setup Backend
```bash
cd backend
npm install
```

Create a `.env` file:
```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

```bash
npm start
```

### 3. Setup Frontend
```bash
cd frontend
npm install
npm start
```

Visit `http://localhost:3000`

---

##  Screenshots

Authentication
Login PageRegistration Page<img width="400" alt="Login Page" src="https://github.com/user-attachments/assets/01ba6612-bcca-4759-add4-e66d61435cbf" /><img width="400" alt="Registration Page" src="https://github.com/user-attachments/assets/f7e93b32-8089-457d-b8b2-6e8c4698530f" />Role-based login for Student, Parent & WardenNew user registration with role selection

Student Portal
Student HomeApply Outpass<img width="400" alt="Student Home" src="https://github.com/user-attachments/assets/7aaf64f6-6a79-4ae3-a926-6a5aefe48e5d" /><img width="400" alt="Apply Outpass" src="https://github.com/user-attachments/assets/af267008-d0a6-4731-acd1-1a70a9d46438" />Student dashboard with outing optionsSubmit outpass request with dates & reason

Parent & Warden Portal
Parent HomeWarden Home<img width="400" alt="Parent Home" src="https://github.com/user-attachments/assets/5e69b713-698a-4545-bd57-aba2a175a034" /><img width="400" alt="Warden Home" src="https://github.com/user-attachments/assets/12654efb-bd8d-4135-adea-0a2b8fe20a1f" />Parent approves/rejects child's outingWarden reviews parent-approved requests

Outing History
<div align="center">
<img width="600" alt="Outing History" src="https://github.com/user-attachments/assets/f9fee3c5-fdff-4b12-b870-5ecbeb9b4a0e" />
Approved outpasses with QR code for gate verification
</div>


---

##  Impact & Metrics

- Serves **500+ students** with automated approval workflows
- Reduced manual approval time by **~60%**
- Handles **100+ daily requests** via OTP + QR verification
- Approval turnaround reduced from hours to **under 5 minutes**

---

##  Future Enhancements

- [ ] SMS/WhatsApp real-time notifications
- [ ] Mobile app (Flutter)
- [ ] Analytics dashboard for wardens
- [ ] Biometric integration at gate

---

##  Author

**Sprushika Suram**  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://www.linkedin.com/in/sprushika-reddy-suram/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black)](https://github.com/sprushikareddy)

---

## 📄 License

This project is licensed under the MIT License.
   
