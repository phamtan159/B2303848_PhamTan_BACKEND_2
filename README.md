# Task Management Frontend

**Project Name**: CT240_NLXD_Phan_Mem_Nhom_3  
**Course**: Software Engineering Principles (CT240)  
**Team**: Team 3  
**Developer**: Phạm Tấn  
**Semester**: II, Academic Year 2025-2026  
**Completion Date**: March 2026

## Project Description

The frontend is a modern web interface for a team task management application. It is built with **Vue.js 3** (Composition API) and **Vuetify**, and it connects to the backend (Spring Boot) via REST API. The interface uses a clean, glassmorphism-inspired design that focuses on usability.

### Key Features:

- **Authentication & Authorization**: Register, login with JWT, and enforce role-based access control for Admin, Manager, and Member.
- **Dashboard**:
  - **Admin**: Overview of users, projects, and tasks, including project status charts.
  - **Member**: Personal task summary, joined projects, and upcoming deadlines.
- **Project Management**:
  - Create, update, and delete projects.
  - Manage project team members: add members, approve join requests, and assign roles (Owner, Manager, Member).
  - Set project visibility to Public or Private.
- **Task Management**:
  - Create, edit, and delete tasks.
  - Assign tasks, set priorities, and define deadlines.
  - Update task status (To Do, In Progress, Done, Cancelled).
- **Collaboration & Interaction**:
  - Add comments to tasks with a rich text editor.
  - Attach files to comments.
- **User Management (Admin)**: View user lists, search users, lock or unlock accounts, and manage roles.
- **Notification System**:
  - Receive alerts for assigned tasks, deadline reminders, and project updates.
  - Project managers can approve or reject membership requests from the notification panel.
  - Mark notifications as read or unread.
- **Reporting & Analytics**:
  - Visual charts to monitor project progress and task distribution.
  - Performance metrics for completion rates and overdue tasks.
  - Export detailed reports to PDF, Excel, or CSV formats.
- **User Profile**: Update personal information and profile avatar.

## Technology Stack

- **Framework**: Vue.js 3 (Composition API + `<script setup>`)
- **UI Library**: Vuetify 3
- State Management: Pinia
- Routing: Vue Router 4
- HTTP Client: Axios
- Rich Text Editor: VueQuill
- Notifications: SweetAlert2
- Build Tool: Vite
- Linting and Formatting: ESLint + Prettier
- IDE: VS Code (with Volar extension)
- Package Manager: npm

## Folder Structure

```text
src
 ┣ api
 ┃ ┣ index.js
 ┃ ┣ projectApi.js
 ┃ ┗ userApi.js
 ┣ components
 ┃ ┣ ProjectCard.vue
 ┃ ┗ UserAvatarName.vue
 ┣ layouts
 ┃ ┣ AdminLayout.vue
 ┃ ┗ MemberLayout.vue
 ┣ router
 ┃ ┗ index.js
 ┣ stores
 ┃ ┣ auth.js
 ┃ ┣ project.js
 ┃ ┣ task.js
 ┃ ┗ user.js
 ┣ views
 ┃ ┣ admin
 ┃ ┃ ┣ AdminDashboard.vue
 ┃ ┃ ┣ NotificationManagement.vue
 ┃ ┃ ┣ ProjectManagement.vue
 ┃ ┃ ┣ ReportDetail.vue
 ┃ ┃ ┣ ReportManagement.vue
 ┃ ┃ ┣ TaskManagement.vue
 ┃ ┃ ┗ UserManagement.vue
 ┃ ┣ auth
 ┃ ┃ ┣ Login.vue
 ┃ ┃ ┗ Register.vue
 ┃ ┣ member
 ┃ ┃ ┣ notifications
 ┃ ┃ ┃ ┗ NotificationList.vue
 ┃ ┃ ┣ project
 ┃ ┃ ┃ ┣ MyProjectList.vue
 ┃ ┃ ┃ ┣ ProjectDetail.vue
 ┃ ┃ ┃ ┣ ProjectForm.vue
 ┃ ┃ ┃ ┗ ProjectList.vue
 ┃ ┃ ┣ task
 ┃ ┃ ┃ ┣ TaskDetail.vue
 ┃ ┃ ┃ ┗ TaskList.vue
 ┃ ┃ ┗ MemberDashboard.vue
 ┃ ┗ profile
 ┃ ┃ ┣ ProfileEdit.vue
 ┃ ┃ ┗ ProfileView.vue
 ┣ App.vue
 ┣ main.js
```

## Local Setup

Requirements:
- Node.js 18+ (LTS recommended)
- npm 9+ (or pnpm/yarn)
- Backend running at `http://localhost:8080`
