<div align="center">

  <img src="docs/assets/light_logo.svg" alt="Learnify Logo" width="400" />

  <br />
  <br />

  ### The Modern Learning Management System

  [![Live Demo](https://img.shields.io/badge/Live_Demo-learnifyplatform.online-00CA58?style=for-the-badge)](https://learnifyplatform.online)
  [![.NET](https://img.shields.io/badge/.NET-9.0-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)](https://dotnet.microsoft.com/)
  [![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://reactjs.org/)
  [![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)](https://www.microsoft.com/sql-server)
  [![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)

  <p align="center">
    <strong>A production-ready, full-stack e-learning platform connecting educators with students worldwide.</strong>
  </p>

  <p align="center">
    <a href="https://learnifyplatform.online"><img src="docs/assets/icons/link.png" width="16" /> Live Demo</a> •
    <a href="#features">Features</a> •
    <a href="#architecture">Architecture</a> •
    <a href="#screenshots">Screenshots</a> •
    <a href="#tech-stack">Tech Stack</a>
  </p>

</div>

---

## 📖 Overview

**Learnify** is a comprehensive Learning Management System (LMS) designed to bridge the gap between educators and students. Built with modern technologies and production-ready architecture, it provides:

- <img src="docs/assets/icons/monitor-play.png" width="16" /> **Live & Recorded Courses** — Support for scheduled live sessions and on-demand video content
- <img src="docs/assets/icons/credit-card.png" width="16" /> **Secure Payments** — Individual and group enrollment with discount options
- <img src="docs/assets/icons/clipboard.png" width="16" /> **Analytics Dashboards** — For both educators and administrators
- <img src="docs/assets/icons/mail.png" width="16" /> **Automated Communications** — Template-based email notifications for all platform events
- <img src="docs/assets/icons/lock.png" width="16" /> **Enterprise Security** — JWT authentication, role-based access, and OTP verification

---

## <img src="docs/assets/icons/lightbulb.png" width="24" /> Features

<table>
<tr>
<td width="50%" valign="top">

### <img src="docs/assets/icons/graduation-cap.png" width="20" /> Student Experience
- **Course Discovery** — Advanced search with category, price, and rating filters
- **Interactive Learning** — Video player with chapter navigation and progress tracking
- **Group Enrollments** — Invite friends for discounted group pricing
- **Reviews & Ratings** — Community feedback system
- **Personal Dashboard** — Track enrolled courses and resume learning

</td>
<td width="50%" valign="top">

### <img src="docs/assets/icons/user.png" width="20" /> Educator Experience
- **Course Builder** — Rich content creation with chapters and video lectures
- **Live Sessions** — Schedule and manage real-time classes
- **Analytics** — Track enrollments, revenue, and student engagement
- **Income Management** — Request payout statements
- **Public Profile** — Showcase courses and build teaching brand

</td>
</tr>
<tr>
<td colspan="2">

### <img src="docs/assets/icons/shield.png" width="20" /> Admin Capabilities
- **User Management** — Complete oversight of all accounts with ban/delete controls
- **Content Moderation** — Review and approve courses before publishing
- **Enrollment Control** — Manage, cancel, or refund student enrollments
- **Platform Analytics** — High-level insights into platform health

</td>
</tr>
</table>

---

## <img src="docs/assets/icons/refresh-ccw.png" width="24" /> Architecture

Learnify follows a **clean client-server architecture** enabling independent scaling and development.

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                              CLIENT LAYER                                   │
│  ┌───────────────────────────────────────────────────────────────────────┐  │
│  │                    React 18 SPA (Vite + Tailwind)                     │  │
│  │       • Component-based UI        • Context State Management          │  │
│  │       • Axios HTTP Client         • React Router Navigation           │  │
│  └───────────────────────────────────────────────────────────────────────┘  │
└─────────────────────────────────────┬───────────────────────────────────────┘
                                      │ HTTPS / REST API
┌─────────────────────────────────────▼───────────────────────────────────────┐
│                              SERVER LAYER                                   │
│  ┌───────────────────────────────────────────────────────────────────────┐  │
│  │                    ASP.NET Core 9 Web API                             │  │
│  │       • RESTful Controllers       • JWT Authentication                │  │
│  │       • Service Layer             • Entity Framework Core             │  │
│  │       • Email Templates           • File Upload Handling              │  │
│  └───────────────────────────────────────────────────────────────────────┘  │
└─────────────────────────────────────┬───────────────────────────────────────┘
                                      │ EF Core ORM
┌─────────────────────────────────────▼───────────────────────────────────────┐
│                               DATA LAYER                                    │
│  ┌───────────────────────────────────────────────────────────────────────┐  │
│  │                      Microsoft SQL Server                             │  │
│  │       • Users & Authentication    • Courses & Content                 │  │
│  │       • Enrollments & Progress    • Payments & Reviews                │  │
│  └───────────────────────────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────────────────────────┘
```

### Deployment Architecture

```
                    ┌──────────────────┐
                    │   Azure Cloud    │
                    └────────┬─────────┘
                             │
          ┌──────────────────┼──────────────────┐
          │                  │                  │
          ▼                  ▼                  ▼
   ┌─────────────┐    ┌─────────────┐    ┌─────────────┐
   │  Frontend   │    │   Backend   │    │  Database   │
   │   (Static)  │    │  (App Svc)  │    │ (SQL Server)│
   └─────────────┘    └─────────────┘    └─────────────┘
```

---

## <img src="docs/assets/icons/monitor-play.png" width="24" /> Screenshots

<div align="center">

### <img src="docs/assets/icons/link.png" width="20" /> Homepage
*Modern hero section with course search and discovery*

<!-- TODO: Add homepage screenshot -->
<!-- ![Homepage](docs/screenshots/homepage.png) -->

<br />

### <img src="docs/assets/icons/book-marked.png" width="20" /> Course Catalog
*Browse and filter through available courses with advanced search capabilities*

<!-- TODO: Add course list screenshot -->
<!-- ![Course List](docs/screenshots/course-list.png) -->

<br />

### <img src="docs/assets/icons/book-marked.png" width="20" /> Course Details
*Detailed course information with live session countdown and enrollment options*

<!-- TODO: Add course detail screenshot -->
<!-- ![Course Details](docs/screenshots/course-detail.png) -->

<br />

### <img src="docs/assets/icons/user.png" width="20" /> Educator Dashboard
*Analytics overview with enrollments, earnings, and course management*

<!-- TODO: Add educator dashboard screenshot -->
<!-- ![Educator Dashboard](docs/screenshots/educator-dashboard.png) -->

<br />

### <img src="docs/assets/icons/clipboard.png" width="20" /> Course Management
*Create and manage courses with chapters and video lectures*

<!-- TODO: Add educator courses screenshot -->
<!-- ![Educator Courses](docs/screenshots/educator-courses.png) -->

<br />

### <img src="docs/assets/icons/graduation-cap.png" width="20" /> Student Enrollments
*Track enrolled courses and learning progress*

<!-- TODO: Add student enrollments screenshot -->
<!-- ![Student Enrollments](docs/screenshots/student-enrollments.png) -->

<br />

### <img src="docs/assets/icons/monitor-play.png" width="20" /> Video Player
*Interactive learning interface with chapter navigation and progress tracking*

<!-- TODO: Add video player screenshot -->
<!-- ![Video Player](docs/screenshots/video-player.png) -->

<br />

### <img src="docs/assets/icons/shield.png" width="20" /> Admin Panel
*User management and platform oversight*

<!-- TODO: Add admin dashboard screenshot -->
<!-- ![Admin Dashboard](docs/screenshots/admin-dashboard.png) -->

</div>

---

## <img src="docs/assets/icons/notebook-pen.png" width="24" /> Tech Stack

| Layer | Technologies |
|-------|-------------|
| **Frontend** | React 18, Vite, Tailwind CSS, Axios, React Router, Framer Motion |
| **Backend** | .NET 9, ASP.NET Core Web API, Entity Framework Core, MailKit |
| **Database** | Microsoft SQL Server |
| **Authentication** | JWT (JSON Web Tokens), OTP Email Verification |
| **UI Components** | PrimeReact, Lucide Icons, React Toastify, Recharts |
| **Video** | React YouTube Player, Custom Progress Tracking |
| **Rich Text** | Quill Editor |
| **CI/CD** | GitHub Actions, Azure App Service |

---

## <img src="docs/assets/icons/lock.png" width="24" /> Security Features

| Feature | Implementation |
|---------|---------------|
| **Authentication** | JWT tokens with configurable expiration |
| **Password Security** | BCrypt hashing with salt |
| **Email Verification** | OTP-based account activation |
| **Authorization** | Role-based access control (Student, Educator, Admin) |
| **API Security** | CORS policies, HTTPS enforcement |
| **Data Protection** | Parameterized queries via EF Core |

---

## <img src="docs/assets/icons/mail.png" width="24" /> Communication System

Learnify includes a comprehensive **template-based email system** for all platform events:

| Category | Email Types |
|----------|-------------|
| **Authentication** | Verification OTP, Welcome, Password Reset |
| **Enrollment** | Confirmation, Group Invitations, Cancellation, Refund |
| **Educator** | Course Approval/Rejection, Income Statements |
| **Support** | Contact Form Acknowledgment, Ticket Notifications |

---

## <img src="docs/assets/icons/users.png" width="24" /> User Roles & Permissions

```
┌─────────────────────────────────────────────────────────────────┐
│                         ADMIN                                   │
│  • Full system access     • User management                     │
│  • Content moderation     • Enrollment control                  │
├─────────────────────────────────────────────────────────────────┤
│                        EDUCATOR                                 │
│  • Create/edit courses    • View analytics                      │
│  • Manage content         • Request payouts                     │
├─────────────────────────────────────────────────────────────────┤
│                        STUDENT                                  │
│  • Browse courses         • Enroll & pay                        │
│  • Track progress         • Leave reviews                       │
└─────────────────────────────────────────────────────────────────┘
```

---

## <img src="docs/assets/icons/clipboard.png" width="24" /> Data Models (Simplified)

```
User ─────────┬───────── Enrollment ─────────── Course
              │                                   │
              │                                   ├── Chapter
              │                                   │      └── Video
              │                                   │
              └───────── Review ──────────────────┘
```

**Key Entities:**
- **User** — Account info, role, profile
- **Course** — Title, description, pricing, status
- **Chapter** — Course sections with ordering
- **Video** — Individual lessons with metadata
- **Enrollment** — Student-course relationship with payment status
- **Review** — Ratings and feedback

---

## <img src="docs/assets/icons/rocket.png" width="24" /> Live Demo

Experience Learnify in action:

<div align="center">

### <img src="docs/assets/icons/link.png" width="20" /> [learnifyplatform.online](https://learnifyplatform.online)

</div>


---

## <img src="docs/assets/icons/mailbox.png" width="24" /> Contact

Have questions or feedback? We'd love to hear from you!

- <img src="docs/assets/icons/mail.png" width="16" /> **Email**: [support@learnifyplatform.online](mailto:support@learnifyplatform.online)
- <img src="docs/assets/icons/link.png" width="16" /> **Website**: [learnifyplatform.online](https://learnifyplatform.online)

---

<div align="center">

  Made with ❤️ by the **Learnify Team**
  Copyright © 2025 Learnify. All Rights Reserved.

</div>
