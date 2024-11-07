# Zen Class Program Management

A MongoDB-based system to manage users, tasks, attendance, company drives, and mentor-student relationships in the Zen Class program.

## Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Usage](#usage)
- [Database Schema](#database-schema)


## About the Project

This project is part of the Zen Class program, focusing on building a MongoDB database to manage student data, codekata progress, and company drives for placements.
It allows tracking of attendance, task submissions, and mentor-mentee interactions.

## Built using

- MongoDB (with MongoDB Compass)

## Features

- Add and update student attendance and task submission status
- Track company drives for placements
- Query students with advanced filtering options
- Manage mentor-mentee relationships


## Usage

1. Open MongoDB Compass and connect to your MongoDB instance.
2. Import the provided collections:
   - `users`
   - `attendance`
   - `codekata`
   - `tasks`
   - `company_drives`
   - `mentors`

3. For run the following queries:
   ```bash
   db.users.find({ /* your query here */ })


## Database Schema

The MongoDB database contains the following collections:

1. **Users**:
   - `user_id` (ObjectId)
   - `name` (String)
   - `email` (String)
   - `batch` (String)
   - `attendance` (Array of objects)
   - `tasks_submitted` (Array of objects)

2. **Company Drives**:
   - `drive_id` (ObjectId)
   - `company_name` (String)
   - `date` (ISODate)

3. **Mentors**:
   - `mentor_id` (ObjectId)
   - `mentor_name` (String)
   - `mentees` (Array of User IDs)


  
