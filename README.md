🧠 Instagram Data Analysis with SQL
📋 Project Overview

This project simulates an Instagram-style social media platform using SQL to explore complex data relationships between users, photos, comments, likes, tags, and follows.
The goal is to analyze user behavior, engagement, and platform dynamics using pure SQL queries — no external analytics tools.

This project was built entirely from scratch, including:

Database schema design

Data population scripts (INSERT INTO ...)

Analytical SQL queries for business insights

Visual schema diagram (included separately as schema.png)

🧩 Database Schema

The database consists of 7 relational tables:
users, photos, comments, likes, follows, tags, and photo_tags.
CREATE TABLE users (
    id INTEGER AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(255) UNIQUE NOT NULL,
    created_at TIMESTAMP DEFAULT NOW()
);
...
Each table includes foreign key relationships to model real-world Instagram interactions, such as:

Each user can upload multiple photos.

Each photo can receive likes, comments, and tags.

Users can follow each other.

You can view the full schema diagram in schema.png.
