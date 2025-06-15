# Road Defect Detection and Task Allocation System

An AI-powered real-time road hazard detection and task management system built using YOLOv8, Flask, and MySQL. Detects potholes and fallen trees from live video, with dashboards for admin and users to assign and manage tasks.

## Project Title
Pathology of Road Defects: Fallen Trees and Potholes

## Overview

- Detects potholes and fallen trees in real-time using live video feed.
- Uses YOLOv8 model for object detection.
- Flask-based web interface for admin and user dashboards.
- MySQL database for storing users, tasks, and statuses.
- Users can accept or reject tasks.
- Rejected tasks are re-added to admin's dashboard.

## Modules

### User Authentication Module
- Login for admin and users.
- Role-based dashboard access.
- Secure session handling via Flask.
- MySQL stores user credentials.

### Real-Time Video Processing Module
- Live camera feed captured via OpenCV.
- YOLOv8 detects potholes/fallen trees in video frames.
- Detection is continuous and automatic.

### Detection and Analysis Module
- YOLOv8 classifies object type.
- Detected issues pushed to the database.
- Admin dashboard displays unassigned tasks.

### Database Management Module
- MySQL manages:
  - User login info.
  - Unassigned tasks.
  - Task status (pending/accepted/rejected).
- job_allocation.sql file included.

### Notification and Reporting Module
- Admin receives real-time updates after detection.
- Users can accept or reject assigned tasks.
- Dashboards reflect task status instantly.
- Rejected tasks go back to admin panel.

## Technologies Used

- Frontend: HTML, CSS, Bootstrap
- Backend: Python (Flask)
- Video Processing: OpenCV
- Object Detection: YOLOv8
- Database: MySQL (XAMPP)
- Server: Flask development server