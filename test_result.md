# Test Results Summary

This document summarizes the outputs of key MongoDB queries and aggregations executed as part of the EduHub Learning Platform project.

# creating database eduhub_db
created successfully
# creating users_collection with validation rules
Collection(Database(MongoClient(host=['localhost:27017'], document_class=dict, tz_aware=False, connect=True), 'eduhub_db'), 'users_collection')
# creating course_collection with validation rules
Collection(Database(MongoClient(host=['localhost:27017'], document_class=dict, tz_aware=False, connect=True), 'eduhub_db'), 'course_collection')
# creating enrollment_collection with validation rules
Collection(Database(MongoClient(host=['localhost:27017'], document_class=dict, tz_aware=False, connect=True), 'eduhub_db'), 'enrollment_collection')
# creating lesson_collection with validation rules
Collection(Database(MongoClient(host=['localhost:27017'], document_class=dict, tz_aware=False, connect=True), 'eduhub_db'), 'lesson_collection')
# creating assignment_collection with validation rules
Collection(Database(MongoClient(host=['localhost:27017'], document_class=dict, tz_aware=False, connect=True), 'eduhub_db'), 'assignment_collection')
# creating submission_collection with validation rules
Collection(Database(MongoClient(host=['localhost:27017'], document_class=dict, tz_aware=False, connect=True), 'eduhub_db'), 'submission_collection')

# 1.2:design schema document for each collection
user_schema:  successfull
course_schema:  successfull
enrollment_schema:  successfull
lesson_schema:  successfull
assignment_schema:  successfull
submission_schema:  successfull

# Task 2.1:insert data samples
# insert 20 users (mis of students and instructors)
InsertManyResult([ObjectId('684ec19f16b31fb0a3538004'), ObjectId('684ec19f16b31fb0a3538005'), ObjectId('684ec19f16b31fb0a3538006'), ObjectId('684ec19f16b31fb0a3538007'), ObjectId('684ec19f16b31fb0a3538008'), ObjectId('684ec19f16b31fb0a3538009'), ObjectId('684ec19f16b31fb0a353800a'), ObjectId('684ec19f16b31fb0a353800b'), ObjectId('684ec19f16b31fb0a353800c'), ObjectId('684ec19f16b31fb0a353800d'), ObjectId('684ec19f16b31fb0a353800e'), ObjectId('684ec19f16b31fb0a353800f'), ObjectId('684ec19f16b31fb0a3538010'), ObjectId('684ec19f16b31fb0a3538011'), ObjectId('684ec19f16b31fb0a3538012'), ObjectId('684ec19f16b31fb0a3538013'), ObjectId('684ec19f16b31fb0a3538014'), ObjectId('684ec19f16b31fb0a3538015'), ObjectId('684ec19f16b31fb0a3538016'), ObjectId('684ec19f16b31fb0a3538017')], acknowledged=True)

# insert 8 course
InsertManyResult([ObjectId('684e9c7b27e46bb527542cff'), ObjectId('684e9c7b27e46bb527542d00'), ObjectId('684e9c7b27e46bb527542d01'), ObjectId('684e9c7b27e46bb527542d02'), ObjectId('684e9c7b27e46bb527542d03'), ObjectId('684e9c7b27e46bb527542d04'), ObjectId('684e9c7b27e46bb527542d05'), ObjectId('684e9c7b27e46bb527542d06')], acknowledged=True)

# insert 15 enrollments
InsertManyResult([ObjectId('684efd27b83d30de7abe2a3e'), ObjectId('684efd27b83d30de7abe2a3f'), ObjectId('684efd27b83d30de7abe2a40'), ObjectId('684efd27b83d30de7abe2a41'), ObjectId('684efd27b83d30de7abe2a42'), ObjectId('684efd27b83d30de7abe2a43'), ObjectId('684efd27b83d30de7abe2a44'), ObjectId('684efd27b83d30de7abe2a45'), ObjectId('684efd27b83d30de7abe2a46'), ObjectId('684efd27b83d30de7abe2a47'), ObjectId('684efd27b83d30de7abe2a48'), ObjectId('684efd27b83d30de7abe2a49'), ObjectId('684efd27b83d30de7abe2a4a'), ObjectId('684efd27b83d30de7abe2a4b'), ObjectId('684efd27b83d30de7abe2a4c')], acknowledged=True)

# insert 25 lesson
InsertManyResult([ObjectId('684eb46616b31fb0a3537fc7'), ObjectId('684eb46616b31fb0a3537fc8'), ObjectId('684eb46616b31fb0a3537fc9'), ObjectId('684eb46616b31fb0a3537fca'), ObjectId('684eb46616b31fb0a3537fcb'), ObjectId('684eb46616b31fb0a3537fcc'), ObjectId('684eb46616b31fb0a3537fcd'), ObjectId('684eb46616b31fb0a3537fce'), ObjectId('684eb46616b31fb0a3537fcf'), ObjectId('684eb46616b31fb0a3537fd0'), ObjectId('684eb46616b31fb0a3537fd1'), ObjectId('684eb46616b31fb0a3537fd2'), ObjectId('684eb46616b31fb0a3537fd3'), ObjectId('684eb46616b31fb0a3537fd4'), ObjectId('684eb46616b31fb0a3537fd5'), ObjectId('684eb46616b31fb0a3537fd6'), ObjectId('684eb46616b31fb0a3537fd7'), ObjectId('684eb46616b31fb0a3537fd8'), ObjectId('684eb46616b31fb0a3537fd9'), ObjectId('684eb46616b31fb0a3537fda'), ObjectId('684eb46616b31fb0a3537fdb'), ObjectId('684eb46616b31fb0a3537fdc'), ObjectId('684eb46616b31fb0a3537fdd'), ObjectId('684eb46616b31fb0a3537fde'), ObjectId('684eb46616b31fb0a3537fdf')], acknowledged=True)

# insert 10 assignments

InsertManyResult([ObjectId('684ebc3416b31fb0a3537fea'), ObjectId('684ebc3416b31fb0a3537feb'), ObjectId('684ebc3416b31fb0a3537fec'), ObjectId('684ebc3416b31fb0a3537fed'), ObjectId('684ebc3416b31fb0a3537fee'), ObjectId('684ebc3416b31fb0a3537fef'), ObjectId('684ebc3416b31fb0a3537ff0'), ObjectId('684ebc3416b31fb0a3537ff1'), ObjectId('684ebc3416b31fb0a3537ff2')], acknowledged=True)

# insert 12 assignment submissions
InsertManyResult([ObjectId('684ebc6c16b31fb0a3537ff3'), ObjectId('684ebc6c16b31fb0a3537ff4'), ObjectId('684ebc6c16b31fb0a3537ff5'), ObjectId('684ebc6c16b31fb0a3537ff6'), ObjectId('684ebc6c16b31fb0a3537ff7'), ObjectId('684ebc6c16b31fb0a3537ff8'), ObjectId('684ebc6c16b31fb0a3537ff9'), ObjectId('684ebc6c16b31fb0a3537ffa'), ObjectId('684ebc6c16b31fb0a3537ffb'), ObjectId('684ebc6c16b31fb0a3537ffc'), ObjectId('684ebc6c16b31fb0a3537ffd'), ObjectId('684ebc6c16b31fb0a3537ffe')], acknowledged=True)
 
 #3.1: create operation
 # add new student
{
  "_id": {
    "$oid": "684eda04b83d30de7abe2a3b"
  },
  "userId": "5b2b1136-89cb-4efb-8aee-763fb14d6d61",
  "email": "lisa@gmail.com",
  "firstName": "lisa",
  "lastName": "aniebo",
  "role": "student",
  "dateJoined": {
    "$date": "2025-06-15T15:34:44.449Z"
  },
  "profile": {
    "bio": "she is a female",
    "avatar": "https://picsum.photos/848/299",
    "skills": [
      "Food technologist",
      "Dancer"
    ]
  },
  "isActive": true
},
 # add new course
{
  "_id": {
    "$oid": "684edb04b83d30de7abe2a3d"
  },
  "courseId": "course_e02e5e51",
  "title": "economy",
  "description": "Sit eye receive bill. Tax may bed top himself base seat. Rate science everybody Mrs mention popular maintain.",
  "instructorId": "instructor_004",
  "category": "business",
  "level": "beginner",
  "duration": 7.7,
  "price": 152.93,
  "tags": [
    "value",
    "well",
    "act"
  ],
  "createdAt": {
    "$date": "2025-06-15T15:39:00.776Z"
  },
  "updatedAt": {
    "$date": "2025-06-15T15:39:00.776Z"
  },
  "isPublished": true,
  "rating": 3.3
},
 # add new enrollment
{
  "_id": {
    "$oid": "685083fd21af983de35f7aa5"
  },
  "enrollmentId": "ENR_1f7714f5",
  "studentId": "8b696369-2d74-4d7c-90f3-f6bc94fd01ca",
  "courseId": "course_b03266ea",
  "enrollmentAt": {
    "$date": "2025-06-16T21:52:13.110Z"
  },
  "status": "active",
  "progress": 0
}
 # add new lesson
 {
  "_id": {
    "$oid": "685084d621af983de35f7aa6"
  },
  "lessonId": "lesson_c25d7c28",
  "courseId": "course_b03266ea",
  "title": "Health hotel enjoy over option than.",
  "description": "Little care second right front response. Senior difficult alone style thank doctor choice.",
  "content": "Assume common particular person community wall. Hit left despite argue likely.\nThird use option already under. Red discover relate ok affect avoid actually.",
  "videoUrl": "http://www.johnson.com/",
  "resources": [
    "http://www.hall.biz/",
    "http://stevens.biz/"
  ],
  "durationMinutes": 16,
  "order": 1,
  "status": "published",
  "isFreePreview": false,
  "createdAt": {
    "$date": "2025-06-16T21:55:50.895Z"
  },
  "updatedAt": {
    "$date": "2025-06-16T21:55:50.895Z"
  }
}
 #3.3 -read operation
 # find all active students
 [{'_id': ObjectId('684ec19f16b31fb0a3538005'), 'userId': 'febc251a-cd99-425b-8031-3c30ba1dfd3f', 'email': 'garywilliams@example.net', 'firstName': 'Timothy', 'lastName': 'Harper', 'role': 'student', 'dateJoined': datetime.datetime(2025, 1, 23, 20, 6, 3), 'profile': {'bio': 'Pm almost world run.', 'avatar': 'https://placekitten.com/62/388', 'skills': ['Comptroller', 'Volunteer coordinator', 'Visual merchandiser']}, 'isActive': True}, {'_id': ObjectId('684ec19f16b31fb0a3538006'), 'userId': '6dc1e62b-e92d-42cd-9e39-0d3d162d939b', 'email': 'barreraemily@example.com', 'firstName': 'Laurie', 'lastName': 'Krueger', 'role': 'student', 'dateJoined': datetime.datetime(2025, 6, 7, 22, 58, 8), 'profile': {'bio': 'Behavior front feeling our side reduce newspaper.', 'avatar': 'https://dummyimage.com/653x1020', 'skills': ['Community pharmacist', 'Manufacturing systems engineer', 'Actuary']}, 'isActive': True}, {'_id': ObjectId('684ec19f16b31fb0a3538009'), 'userId': 'c9ea4e17-37b4-4e96-b19d-8b2f069d28f0', 'email': 'qpeck@example.com', 'firstName': 'John', 'lastName': 'Garrett', 'role': 'student', 'dateJoined': datetime.datetime(2025, 1, 3, 0, 29, 37), 'profile': {'bio': 'Part once one speak bar.', 'avatar': 'https://dummyimage.com/346x492', 'skills': ['Investment banker, corporate', 'Homeopath']}, 'isActive': True}, {'_id': ObjectId('684ec19f16b31fb0a353800d'), 'userId': '4ba15184-8c3f-48a9-89ae-5a1455c896b7', 'email': 'egomez@example.org', 'firstName': 'Wesley', 'lastName': 'Williamson', 'role': 'student', 'dateJoined': datetime.datetime(2025, 5, 21, 12, 39, 18), 'profile': {'bio': 'Explain return production national husband.', 'avatar': 'https://picsum.photos/44/662', 'skills': ['Mining engineer', 'Radio producer', 'Presenter, broadcasting']}, 'isActive': True}, {'_id': ObjectId('684ec19f16b31fb0a3538012'), 'userId': '54696721-633f-4a88-9a4a-3ee209907615', 'email': 'lydia51@example.net', 'firstName': 'Kathleen', 'lastName': 'Thompson', 'role': 'student', 'dateJoined': datetime.datetime(2025, 2, 11, 19, 34, 28), 'profile': {'bio': 'Whose newspaper growth question care single wonder exactly.', 'avatar': 'https://placekitten.com/372/258', 'skills': ['Furniture designer', 'Producer, television/film/video']}, 'isActive': True}, {'_id': ObjectId('684ec43f16b31fb0a353801f'), 'userId': '4dab405f-dd1b-494c-b694-38d0f0c7ec00', 'email': 'michaelmendez@example.net', 'firstName': 'Taylor', 'lastName': 'Wells', 'role': 'student', 'dateJoined': datetime.datetime(2025, 6, 15, 14, 1, 51, 189000), 'profile': {'bio': 'Assume interest among director try.', 'avatar': 'https://picsum.photos/324/839', 'skills': ['Garment/textile technologist', 'Health physicist']}, 'isActive': True}]

6
 # retrieve course details with instructor
{'_id': ObjectId('684ec6a816b31fb0a3538020'), 'courseId': 'course_34d5c75b', 'title': 'Leg despite', 'description': 'Which gas however friend town. Art response remember company.', 'instructorId': '75e9ac6f-8f15-443b-aa67-737b0ae2b700', 'category': 'Programming', 'level': 'beginner', 'duration': 4.4, 'price': 147.81, 'tags': ['own', 'method', 'through'], 'createdAt': datetime.datetime(2025, 6, 15, 14, 12, 8, 724000), 'updatedAt': datetime.datetime(2025, 6, 15, 14, 12, 8, 724000), 'isPublished': True, 'instructorInfo': {'_id': ObjectId('684ec19f16b31fb0a353800a'), 'userId': '75e9ac6f-8f15-443b-aa67-737b0ae2b700', 'email': 'danielbarber@example.net', 'firstName': 'Ashley', 'lastName': 'Wood', 'role': 'instructor', 'dateJoined': datetime.datetime(2025, 4, 24, 3, 34, 43), 'profile': {'bio': 'Growth south already down parent.', 'avatar': 'https://placekitten.com/596/231', 'skills': ['Race relations officer']}, 'isActive': True}}

# get all courses in a specific category

[{'_id': ObjectId('684e9c7b27e46bb527542d00'), 'courseId': 'course_2', 'title': 'Bill foot church operation skill', 'description': 'Trade nation us pick detail forget really suffer.', 'instructorId': '5f07738c-9e82-4a2f-ba23-287654e3ae7e', 'category': 'Programming', 'level': 'beginner', 'duration': 9.5, 'price': 119.97, 'tags': ['property', 'my', 'discover'], 'createdAt': datetime.datetime(2025, 6, 12, 12, 48, 27), 'updatedAt': datetime.datetime(2025, 6, 15, 11, 9, 25), 'isPublished': True}, {'_id': ObjectId('684e9c7b27e46bb527542d04'), 'courseId': 'course_6', 'title': 'These enough never', 'description': 'Whether wear how one. Determine add find. If member born color argue.', 'instructorId': '45afd089-eca4-4216-803a-589d94decd65', 'category': 'Programming', 'level': 'advanced', 'duration': 1.8, 'price': 66.28, 'tags': ['order', 'reduce', 'seven'], 'createdAt': datetime.datetime(2024, 11, 28, 2, 54, 25), 'updatedAt': datetime.datetime(2025, 6, 15, 11, 8, 39), 'isPublished': False}, {'_id': ObjectId('684e9c7b27e46bb527542d05'), 'courseId': 'course_7', 'title': 'Wind usually myself see', 'description': 'Where civil south left small edge. Close woman traditional listen. Allow finish radio.', 'instructorId': '45afd089-eca4-4216-803a-589d94decd65', 'category': 'Programming', 'level': 'beginner', 'duration': 8.9, 'price': 7.65, 'tags': ['necessary', 'suffer', 'actually', 'employee'], 'createdAt': datetime.datetime(2025, 3, 22, 0, 54, 42), 'updatedAt': datetime.datetime(2025, 6, 15, 11, 10, 31), 'isPublished': False}, {'_id': ObjectId('684ec6a816b31fb0a3538020'), 'courseId': 'course_34d5c75b', 'title': 'Leg despite', 'description': 'Which gas however friend town. Art response remember company.', 'instructorId': '75e9ac6f-8f15-443b-aa67-737b0ae2b700', 'category': 'Programming', 'level': 'beginner', 'duration': 4.4, 'price': 147.81, 'tags': ['own', 'method', 'through'], 'createdAt': datetime.datetime(2025, 6, 15, 14, 12, 8, 724000), 'updatedAt': datetime.datetime(2025, 6, 15, 14, 12, 8, 724000), 'isPublished': True}]

# find students enrolled in a particular course

Student IDs found in enrollment: ['ff296f63-308d-465b-bd79-55eebdb2abc9']
Matching users found: 1

Students enrolled in course 'course_8':
John Mcgee

# search course by title
Searching titles for: ask
Courses matching 'ask':
- Ask yourself event

#3.3- update operations
# updaate a users profile information
Documents updated: 1
# mark a course as published
UpdateResult({'n': 1, 'nModified': 1, 'ok': 1.0, 'updatedExisting': True}, acknowledged=True)
# update assignment grades
UpdateResult({'n': 1, 'nModified': 1, 'ok': 1.0, 'updatedExisting': True}, acknowledged=True)
Updated submission sub_3 successfully.
# add tags to an existing course
UpdateResult({'n': 1, 'nModified': 1, 'ok': 1.0, 'updatedExisting': True}, acknowledged=True)
Tags added successfully.

# 3.4 - delete operations
# remove a user(soft delete)
Soft deleted: UpdateResult({'n': 1, 'nModified': 1, 'ok': 1.0, 'updatedExisting': True}, acknowledged=True)
# delete an enrollment
Enrollment deleted: DeleteResult({'n': 1, 'ok': 1.0}, acknowledged=True)
# remove a lesson from a course
Lesson deleted: DeleteResult({'n': 1, 'ok': 1.0}, acknowledged=True)

# task4 -advanceed queries aggregation
# 4.1 - complex queries
# find courses with price $50 and $200
Courses found: 8
# get userswho joined in the last 6 months
Recent users: 21
# find courses that have specific tags using $in operator
Courses found: 2
course_4 - Ask yourself event
course_6 - These enough never
# retrieve assignments with due dates in the next week
Upcoming assignments in the next 7 days: 4
- Party usually really middle any. | Due: 2025-06-17 14:27:20
- Win project agree air forward election sort form. | Due: 2025-06-22 15:45:32
- Fill democratic old theory even red. | Due: 2025-06-17 15:54:43
- Arrive opportunity see. | Due: 2025-06-19 07:15:14

# 4.2-aggregation pipeline
  #course enrollment
    #[{'_id': 'course_4', 'totalEnrollments': 4}, {'_id': 'course_e02e5e51', 'totalEnrollments': 2}, {'_id': 'course_2', 'totalEnrollments': 2}, {'_id': 'course_3', 'totalEnrollments': 2}, {'_id': 'course_7', 'totalEnrollments': 2}, {'_id': 'course_5', 'totalEnrollments': 1}, {'_id': 'course_1', 'totalEnrollments': 1}, {'_id': 'course_8', 'totalEnrollments': 1}]
     count total enrollment per course
    
    #calculate average course rating
    [{'_id': 'course_8', 'averageRating': 4.3}, {'_id': 'course_4', 'averageRating': 3.35}, {'_id': 'course_3', 'averageRating': 3.0}, {'_id': 'course_e02e5e51', 'averageRating': 2.9}, {'_id': 'course_5', 'averageRating': 2.5}, {'_id': 'course_2', 'averageRating': 1.9000000000000001}, {'_id': 'course_7', 'averageRating': 1.5}, {'_id': 'course_1', 'averageRating': 1.5}]
    #group by course category
    [{'_id': 'Business', 'courseCount': 4, 'averagePrice': 115.88}, {'_id': 'Programming', 'courseCount': 3, 'averagePrice': 64.63333333333334}, {'_id': 'Data Science', 'courseCount': 1, 'averagePrice': 189.69}, {'_id': 'business', 'courseCount': 1, 'averagePrice': 152.93}]

# student performance analysis
  # average grade per student
  [{'_id': '37f3a269-f0f1-4082-8914-3ec5ecfe746b', 'averageScore': 60.333333333333336, 'submissionsCount': 3}, {'_id': 'c138ab1c-af4a-4414-b8a0-547fda28c0b0', 'averageScore': 59.0, 'submissionsCount': 1}, {'_id': '895f1d23-09ad-4211-ad98-476c69fc9339', 'averageScore': 44.0, 'submissionsCount': 1}, {'_id': 'e3b6a3ab-86d9-4c98-b092-6d9e30c15e9e', 'averageScore': 42.0, 'submissionsCount': 1}, {'_id': '92447918-de57-4256-8d57-b2920bc6173f', 'averageScore': 36.666666666666664, 'submissionsCount': 3}, {'_id': 'bc84b583-6ce7-4c84-b3a9-8bda575c4231', 'averageScore': 36.0, 'submissionsCount': 1}, {'_id': 'fc3c841a-1396-4d02-bda5-56064edb8f51', 'averageScore': 17.0, 'submissionsCount': 1}, {'_id': '1ab9d687-2803-4a74-9c74-6f89d78926d6', 'averageScore': 14.0, 'submissionsCount': 1}]
  # completion rate by course
  [{'_id': 'course_1', 'avgCompletionRate': 75.67}, {'_id': 'course_4', 'avgCompletionRate': 55.81}, {'_id': 'course_e02e5e51', 'avgCompletionRate': 47.705}, {'_id': 'course_3', 'avgCompletionRate': 45.445}, {'_id': 'course_5', 'avgCompletionRate': 42.76}, {'_id': 'course_2', 'avgCompletionRate': 40.37}, {'_id': 'course_8', 'avgCompletionRate': 36.11}, {'_id': 'course_7', 'avgCompletionRate': 34.33}]
  # top  performing student
  [{'_id': '37f3a269-f0f1-4082-8914-3ec5ecfe746b', 'avgScore': 60.333333333333336}, {'_id': 'c138ab1c-af4a-4414-b8a0-547fda28c0b0', 'avgScore': 59.0}, {'_id': '895f1d23-09ad-4211-ad98-476c69fc9339', 'avgScore': 44.0}, {'_id': 'e3b6a3ab-86d9-4c98-b092-6d9e30c15e9e', 'avgScore': 42.0}, {'_id': '92447918-de57-4256-8d57-b2920bc6173f', 'avgScore': 36.666666666666664}]

# instructor analysis
  # total students taught by each instructor
  [{'_id': '10b098d9-9d79-4ebc-a181-27de21fe2639', 'instructorId': '10b098d9-9d79-4ebc-a181-27de21fe2639', 'totalStudents': 4}, {'_id': '5d32c8a0-edc7-4f0d-8315-9ea73b09637d', 'instructorId': '5d32c8a0-edc7-4f0d-8315-9ea73b09637d', 'totalStudents': 2}, {'_id': '2c37eaa8-b73a-4fe1-abe7-71bf93de638e', 'instructorId': '2c37eaa8-b73a-4fe1-abe7-71bf93de638e', 'totalStudents': 1}, {'_id': '45afd089-eca4-4216-803a-589d94decd65', 'instructorId': '45afd089-eca4-4216-803a-589d94decd65', 'totalStudents': 1}, {'_id': '5f07738c-9e82-4a2f-ba23-287654e3ae7e', 'instructorId': '5f07738c-9e82-4a2f-ba23-287654e3ae7e', 'totalStudents': 1}, {'_id': 'bdae559f-2f3a-49af-9b36-22ad2ce3657c', 'instructorId': 'bdae559f-2f3a-49af-9b36-22ad2ce3657c', 'totalStudents': 1}]
  # average course rating per instructor
  [{'_id': None, 'avgRating': 3.8444444444444446}]
  # revenue generated per instructor
  Instructor: None | Revenue: $471.08
Instructor: Bob Smith | Revenue: $239.94
Instructor: Diana Prince | Revenue: $231.0
Instructor: Ethan Hunt | Revenue: $189.69
Instructor: Alice Johnson | Revenue: $183.01
Instructor: Charlie Lee | Revenue: $145.68
  Instructor names updated for courses.
# advancced analysis
  # monthly enrollment trend
[{'_id': {'year': None, 'month': None}, 'totalEnrollments': 15}]
  # most popular course categories
[{'_id': 'Business', 'totalEnrollments': 8}, {'_id': 'Programming', 'totalEnrollments': 4}, {'_id': 'business', 'totalEnrollments': 2}, {'_id': 'Data Science', 'totalEnrollments': 1}]
  # students engagement metrics
  [{'_id': None, 'avgSubmissionsPerStudent': 1.5}]

#task5 - indexing and performance
#5.1
# user email look up
'email_1'
# course search by title and category
'category_1'
# Assignment queries by due date
'dueDate_1'
# enrollment queries by student and course
'studentId_1_courseId_1'
# 5.2- query optimization
# analyse query performance using explain() method  in pymongo
1*-
{'explainVersion': '1', 'queryPlanner': {'namespace': 'eduhub_db.users_collection', 'indexFilterSet': False, 'parsedQuery': {'email': {'$eq': 'lisa@example.com'}}, 'queryHash': 'DFF5CD1D', 'planCacheKey': 'D871B341', 'maxIndexedOrSolutionsReached': False, 'maxIndexedAndSolutionsReached': False, 'maxScansToExplodeReached': False, 'winningPlan': {'stage': 'FETCH', 'inputStage': {'stage': 'IXSCAN', 'keyPattern': {'email': 1}, 'indexName': 'email_1', 'isMultiKey': False, 'multiKeyPaths': {'email': []}, 'isUnique': True, 'isSparse': False, 'isPartial': False, 'indexVersion': 2, 'direction': 'forward', 'indexBounds': {'email': ['["lisa@example.com", "lisa@example.com"]']}}}, 'rejectedPlans': []}, 'executionStats': {'executionSuccess': True, 'nReturned': 0, 'executionTimeMillis': 212, 'totalKeysExamined': 0, 'totalDocsExamined': 0, 'executionStages': {'stage': 'FETCH', 'nReturned': 0, 'executionTimeMillisEstimate': 0, 'works': 1, 'advanced': 0, 'needTime': 0, 'needYield': 0, 'saveState': 1, 'restoreState': 1, 'isEOF': 1, 'docsExamined': 0, 'alreadyHasObj': 0, 'inputStage': {'stage': 'IXSCAN', 'nReturned': 0, 'executionTimeMillisEstimate': 0, 'works': 1, 'advanced': 0, 'needTime': 0, 'needYield': 0, 'saveState': 1, 'restoreState': 1, 'isEOF': 1, 'keyPattern': {'email': 1}, 'indexName': 'email_1', 'isMultiKey': False, 'multiKeyPaths': {'email': []}, 'isUnique': True, 'isSparse': False, 'isPartial': False, 'indexVersion': 2, 'direction': 'forward', 'indexBounds': {'email': ['["lisa@example.com", "lisa@example.com"]']}, 'keysExamined': 0, 'seeks': 1, 'dupsTested': 0, 'dupsDropped': 0}}, 'allPlansExecution': []}, 'command': {'find': 'users_collection', 'filter': {'email': 'lisa@example.com'}, '$db': 'eduhub_db'}, 'serverInfo': {'host': 'DESKTOP-GTB1LCJ', 'port': 27017, 'version': '6.0.24', 'gitVersion': '1b052b94a23863fd12be97aaa4e4b1d96456e5cc'}, 'serverParameters': {'internalQueryFacetBufferSizeBytes': 104857600, 'internalQueryFacetMaxOutputDocSizeBytes': 104857600, 'internalLookupStageIntermediateDocumentMaxSizeBytes': 104857600, 'internalDocumentSourceGroupMaxMemoryBytes': 104857600, 'internalQueryMaxBlockingSortMemoryUsageBytes': 104857600, 'internalQueryProhibitBlockingMergeOnMongoS': 0, 'internalQueryMaxAddToSetBytes': 104857600, 'internalDocumentSourceSetWindowFieldsMaxMemoryBytes': 104857600}, 'ok': 1.0}

2*-
{'stage': 'COLLSCAN', 'filter': {'$and': [{'dueDate': {'$lte': datetime.datetime(2025, 6, 22, 19, 49, 24, 586000)}}, {'dueDate': {'$gte': datetime.datetime(2025, 6, 15, 19, 49, 24, 586000)}}]}, 'direction': 'forward'}
# optimize at least 3 slow performance
3*-
Explain plan: {'stage': 'FETCH', 'inputStage': {'stage': 'IXSCAN', 'keyPattern': {'dueDate': 1}, 'indexName': 'dueDate_1', 'isMultiKey': False, 'multiKeyPaths': {'dueDate': []}, 'isUnique': False, 'isSparse': False, 'isPartial': False, 'indexVersion': 2, 'direction': 'forward', 'indexBounds': {'dueDate': ['[new Date(1750016964586), new Date(1750621764586)]']}}}
search by email
1*slow
Query time without index: 0.018988847732543945
*optimization
'email_1'
Query time with index: 0.0019998550415039062
2*slow
Time before index: 0.002995729446411133
*optimization
'title_text_category_text'
Time after index: 0.0029969215393066406
3* slow - optimization time
Time taken: 4.091989755630493 seconds

# document the performance improvements using python timing functions

#6.1-
Collection(Database(MongoClient(host=['localhost:27017'], document_class=dict, tz_aware=False, connect=True), 'eduhub_db'), 'users_collection')
# 6.2 - error handling
# Duplicate key errors
Duplicate email detected! Please use a different email.
# invalid data type insertion
inserted successfully
# missing required fields
User inserted successfully.