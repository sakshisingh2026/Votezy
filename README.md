# 🗳️ Votezy — Your Vote, Secured.

> A modern, secure, and efficient online voting platform built to tackle the real challenges of traditional elections.

---

## 💡 The Problem

Traditional voting methods often face:

- ⏳ Long queues and significant waiting times
- 🚫 Limited accessibility for disabled and abroad voters
- 💸 High operational costs and complex logistics
- ⚠️ Risk of human errors and potential malpractice
- 🔒 Concerns about security and transparency

**Votezy solves all of this** — online voting that eliminates queues, is accessible to all, cost-effective, paperless, and fully transparent.

---

## ✨ Key Features

| Feature | Description |
|---|---|
| 🔐 Secure Login System | Role-based access for Voters, Candidates, and Admins |
| 🗳️ Online Voting | Cast votes safely from anywhere, anytime |
| 👤 Voter & Candidate Profiles | Manage personal information and credentials securely |
| 📊 Real-Time Results | Instant and transparent election outcome display |
| 🚫 Duplicate Vote Prevention | One person, one vote — enforced by backend checks |
| 📈 Progress Tracking | Admin dashboard to monitor participation |

---

## 🛡️ Security Measures

- 🔒 **End-to-End Encryption** — All sensitive voter data is encrypted during transmission and storage
- 🛡️ **Role-Based Authentication** — Only authorized users (Voter, Candidate, Admin) can access the system
- 🔑 **Password Encryption** — Passwords stored securely using strong hashing algorithms
- 🚫 **Duplicate Vote Prevention** — Each voter can vote only once, enforced at the backend
- ⛔ **No Admin Self-Registration** — Admin accounts are system-controlled only, not publicly registerable

---

## 🛠️ Tech Stack

**Frontend**
- HTML, CSS, JavaScript

**Backend**
- Spring Boot, Spring MVC, Spring Data JPA, Spring Security

**Database**
- MySQL

---

## 🏗️ System Architecture
```
User Interface  →  Frontend Services (API Gateway & Session Handling)
                          ↓
               Backend Services (Business Logic & Vote Processing)
                          ↓
            Security Module (Authentication, Encryption & Audits)
                          ↓
              Database (Persistent Vote & Audit Storage)
```

---

## 📁 Project Structure
```
Votezy/
├── Backend/                          # Spring Boot REST API
│   └── src/
│       └── main/
│           ├── java/
│           │   └── com/votezy/
│           │       ├── controller/
│           │       ├── service/
│           │       ├── repository/
│           │       ├── model/
│           │       └── security/
│           └── resources/
│               └── application.properties
└── Frontend/
    └── online-votezy-frontend/       # HTML, CSS, JS frontend
        ├── index.html
        ├── style.css
        └── script.js
```

---

## ⚙️ Getting Started

### Prerequisites
- Java 17+
- Maven
- MySQL
- Any modern browser

### 🔧 Backend Setup
```bash
cd Backend
```

Configure your database in `src/main/resources/application.properties`:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/votezy_db
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
```

Then run:
```bash
mvn spring-boot:run
```

### 💻 Frontend Setup
```bash
cd Frontend/online-votezy-frontend
```

Open `index.html` in your browser or use the VS Code **Live Server** extension.

Make sure the API base URL points to `http://localhost:8080`.

---

## 🔗 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/auth/register` | Register a new user |
| POST | `/api/auth/login` | Login |
| GET | `/api/candidates` | Get all candidates |
| POST | `/api/vote` | Cast a vote |
| GET | `/api/results` | View election results |

---

## ✅ Advantages

- 📈 **Increased Voter Participation** — Easy access encourages more people to vote
- 💰 **Cost-Effective** — Reduces expenses related to physical polling stations and staff
- ⚡ **Speed & Accuracy** — Instantaneous and error-free result tabulation
- 🔍 **Enhanced Transparency** — Verifiable and auditable voting process
- 🌱 **Environment Friendly** — Fully paperless system

---

## ⚠️ Known Limitations

- 🌐 **Internet Dependency** — Requires stable connectivity; may exclude remote/underserved areas
- 📱 **Digital Literacy** — Older demographics may find digital platforms challenging
- 🛡️ **Security Risks** — Online systems carry inherent cybersecurity vulnerabilities
- ⚙️ **System Failures** — Technical glitches could disrupt the election process
- 🤝 **Trust Issues** — Some voters may prefer traditional, tangible voting methods

---

## 🚀 Future Enhancements

- 🔏 **Biometric Authentication** — Fingerprint and Face ID for enhanced login security
- ⛓️ **Blockchain Integration** — Tamper-proof and transparent voting records
- 🌍 **Multi-Language Support** — Broader citizen accessibility
- 📱 **Mobile App** — Dedicated apps for convenient voting via smartphones
- 🤖 **AI-Based Analytics** — Real-time insights and advanced fraud detection

---

## 👩‍💻 Author

**Sakshi Singh** — B.Tech CSE Student
[@sakshisingh2026](https://github.com/sakshisingh2026)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

> *"Join us in shaping the future of democracy with Votezy — your vote, secured."*
