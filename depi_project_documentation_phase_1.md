# Mansa Tech (منصتك) - DEPI Graduation Project
**Project Documentation - Phase 1 Submission**

---

## 1. Project Planning & Management

### Project Proposal
* **Overview:** Mansa Tech is an educational management platform designed to connect students, instructors, and system admins. The platform simplifies course management, student progress tracking, and assignment submission in a single web application.
* **Objectives:**
  1. Provide a centralized system for instructors to manage courses and assignments.
  2. Allow students to browse courses, track their learning progress, and submit deliverables easily.
  3. Implement a secure, role-based backend system using .NET Core.
* **Scope:**
  * **Backend:** ASP.NET Core Web API with Entity Framework Core and SQL Server.
  * **Frontend:** Responsive Web UI integrated with backend APIs.
  * **Authentication:** ASP.NET Core Identity with JWT for user login and permissions.

### Project Plan & Timeline
1. **Phase 1: Requirements & Planning (Weeks 1–2)**
   * Finalizing system features, DB design, and API endpoints.
2. **Phase 2: Core Development (Weeks 3–5)**
   * Building DB models, authentication logic, and main API controllers.
3. **Phase 3: Integration & UI Development (Weeks 6–7)**
   * Connecting frontend screens with backend APIs and validating user flows.
4. **Phase 4: Testing & Final Delivery (Week 8)**
   * Bug fixing, API testing via Postman, and GitHub code cleanup.

### Task Assignment & Roles
> *Note: Team roles and individual task assignments will be assigned and updated by the 5 team members.*

* **Team Member 1:** [To be specified by team]
* **Team Member 2:** [To be specified by team]
* **Team Member 3:** [To be specified by team]
* **Team Member 4:** [To be specified by team]
* **Team Member 5:** [To be specified by team]

### Risk Assessment & Mitigation Plan
* **Risk 1: Delays in API and Frontend Integration**
  * *Mitigation:* Document APIs early using Swagger so frontend and backend work can happen in parallel.
* **Risk 2: Database Query Performance**
  * *Mitigation:* Keep LINQ queries simple and avoid unnecessary data loading using basic indexing in SQL Server.
* **Risk 3: User Authorization Issues**
  * *Mitigation:* Implement basic Role-Based Access Control (RBAC) to ensure users can only access their designated views.

### KPIs (Key Performance Indicators)
* **System Stability:** Basic functionality works consistently without application crashes.
* **API Response Time:** APIs respond in a reasonable timeframe (under 500ms for standard requests).
* **Feature Completeness:** Successful implementation of core user flows (Login, Course Browsing, Assignment Submission).

---

## 2. Literature Review

### Feedback & Evaluation
> *Note: This section will be updated after receiving feedback and evaluation from the instructor/lecturer.*

* **Lecturer Assessment:** [Pending Instructor Review]
* **Evaluation Notes:** [Pending Instructor Review]

### Suggested Improvements
1. **Real-time Notifications:** Adding basic notifications using SignalR for new assignments or announcements.
2. **File Storage:** Integrating external storage (like Cloudinary) for uploading PDFs and course materials instead of saving locally.
3. **Caching:** Applying basic caching strategies for static or frequently accessed data like category lists.

---

## 3. Requirements Gathering

### Stakeholder Analysis
1. **Students:** Need an easy way to view enrolled courses, watch lessons, and submit homework.
2. **Instructors:** Need tools to create courses, add content, and grade student submissions.
3. **Admins:** Need simple dashboard access to manage platform users and system settings.

### User Stories & Use Cases
* **As a Student:** I want to create an account and log in so that I can browse available courses.
* **As a Student:** I want to submit my assignments online so that my instructor can review them.
* **As an Instructor:** I want to upload new course modules and assignments for my students.
* **As an Admin:** I want to view active users and courses to ensure the platform operates smoothly.

### Functional Requirements
1. **User Authentication & Authorization:**
   * User registration and login (Student, Instructor, Admin).
   * Password hashing and JWT issuance.
2. **Course Management:**
   * Create, update, and delete courses (Instructors/Admins).
   * View course details and lesson lists (Students).
3. **Enrollment & Progress Tracking:**
   * Enroll students into selected courses.
   * Basic status tracking for completed lessons.
4. **Assignments & Submissions:**
   * Instructors can create assignments with deadlines.
   * Students can upload submissions.

### Non-functional Requirements
1. **Performance:** System pages and endpoints should load within acceptable limits during normal usage.
2. **Security:** Passwords must be hashed using ASP.NET Core Identity standards, and API endpoints secured via tokens.
3. **Usability:** Simple, clean user interface accessible on standard desktop and mobile browsers.
4. **Maintainability:** Code organized logically following clean layered architecture practices.