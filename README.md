# MongoDB Learning Platform Project

This project simulates the backend of an online learning platform using MongoDB and Python. It covers core components such as users, courses, lessons, assignments, enrollments, and submissions — all connected using realistic data relationships.

---

##  Setup Instructions

1. Make sure your MongoDB server is running locally (`mongod`) or manually in your terminal.
2. Install required Python libraries:
   ```bash
   pip install pymongo faker
Open the notebook:

eduhub_mongodb_Project.ipynb
Run the notebook cell-by-cell to set up the database, insert sample data, and execute queries.

# Database Schema
Collection	Description
users_collection	Stores users with fields like userId, name, email, role (student/instructor)
courses_collection	Contains courseId, title, description, and instructor
enrollment_collection	Links students to courses, with enrollmentDate
lesson	Course modules with lessonId, courseId, title
assignment	Linked to lessons or courses with due dates
submission	Tracks student assignment submissions and scores

# Query Examples
Retrieve assignments due within the next 7 days

Calculate average scores for each student

Count enrollments per course

Identify top-performing students by average score

Track submissions per assignment and student

# Performance Analysis
Indexes were created on frequently queried fields such as userId, courseId, and dueDate, improving query speed.

Aggregation pipelines were optimized by using $match, $group, and $sort stages effectively.

Sample queries executed with and without indexes to confirm performance improvement.

# Challenges Faced & Solutions
 1. Handling Invalid Data Types
Some fields (like dates) initially caused errors when invalid or missing.
# Solution: Added try-except blocks and validated data before insertion.

2. Duplicate Faker Data
Faker sometimes generated duplicates, especially for names and emails.
# Solution: Used uniqueness constraints and checked for duplicates during generation.

 3. Debugging Logic Errors
Errors during aggregation or joins were tricky to trace.
# Solution: Stayed calm, isolated each pipeline stage, used helper functions, and printed intermediary results for debugging.

"What helped me the most was organizing code into clear functions, being patient, and debugging step-by-step. Deleting unused variables and carefully reading error messages saved me more than once." – Lisa

# Project Structure
 eduhub-mongodb-project/
├── eduhub_mongodb_Project.ipynb        # Main notebook with queries and outputs
├── eduhub_queries.py                   # Python script with all MongoDB operations
├── sample_data/                        # Exported JSON data from MongoDB collections
├── test_results.md                     # Saved query outputs for testing and review
├── README.md                           # This documentation file
