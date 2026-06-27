# CT240 - Task Management System

A full-stack group task management system built with Spring Boot and Vue.js. Developed as part of the CT240 Software Engineering course.

## 📋 Overview

This project provides a complete task management solution with real-time notifications, role-based access control, and project collaboration features. Backend runs on Spring Boot with MongoDB, frontend built with Vue 3 and Vuetify.

## 🔧 Tech Stack

**Backend** ([CT240_NLXD_Phan_Mem_Nhom_3_BE](CT240_NLXD_Phan_Mem_Nhom_3_BE))

- Java 17, Spring Boot 4.0.3
- MongoDB for data storage
- JWT authentication
- WebSocket (STOMP) for real-time updates
- Design patterns: Observer, Factory, Strategy

**Frontend** ([CT240_NLXD_Phan_Mem_Nhom_3_FE](CT240_NLXD_Phan_Mem_Nhom_3_FE))

- Vue 3 + Vite
- Vuetify for UI components
- Pinia for state management
- Axios for API calls
- Chart.js for analytics

## ✨ Features

- User management with role-based access (Admin, Manager, Member)
- Project creation and team collaboration
- Task assignment and status tracking
- Real-time notifications and comments
- Activity logging and reporting
- File attachment support

## 🚀 Quick Start

### Backend

```bash
cd CT240_NLXD_Phan_Mem_Nhom_3_BE
mvn spring-boot:run
```

Server runs on `http://localhost:8080`

### Frontend

```bash
cd CT240_NLXD_Phan_Mem_Nhom_3_FE
npm install
npm run dev
```

Access at `http://localhost:5173`

## 📂 Project Structure

```
CT240_NLXD_Phan_Mem_Nhom_3_BE/  # Spring Boot backend
CT240_NLXD_Phan_Mem_Nhom_3_FE/  # Vue 3 frontend
```

## � Developer

**Phạm Tấn** - Full Stack Developer
