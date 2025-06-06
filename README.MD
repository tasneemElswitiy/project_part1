# Course Platform Database Schema

This project contains the **Entity Relationship Diagram (ERD)** for a simple online course platform.

## Schema Diagram

The database schema is illustrated in the following image:


> Replace `اسم_الصورة.jpg` with the actual name of your uploaded image file.

---

##  Tables Overview

### User
Stores user account information.
- `id`: Unique user ID
- `user_name`: Username
- `email`: User email
- `password`: Encrypted password

---

### Course
Information about each course.
- `id`: Course ID
- `category_id`: Foreign key to Category table
- `title`: Course title
- `description`: Course description
- `instructor`: Instructor name
- `price`: Course price

---

###  Category
Defines course categories.
- `id`: Category ID
- `name`: Category name

---

###  Enrollment
Tracks which users are enrolled in which courses.
- `id`: Enrollment ID
- `user_id`: User foreign key
- `course_id`: Course foreign key

---

###  Bookmark
Users can bookmark courses.
- `id`: Bookmark ID
- `user_id`: User foreign key
- `course_id`: Course foreign key

---

###  Course Content
Stores individual course sections or lessons.
- `id`: Content ID
- `course_id`: Related course
- `title`: Section title
- `content`: Text or description of the section

---



##  License
This project is open-source and free to use for learning or personal projects.
