# Classroom-Attendance-Management-System

Abstract:

The Classroom Attendance Management that manages attendance records for a classroom using DynamoDB, a NoSQL database. The system allows users to perform various operations, including adding, updating, and deleting attendance records, adding or removing students from a class, and generating attendance reports for both students and classes. This documentation outlines the objectives and functionality of the system, as well as its design and architecture.

Overview:

The attendance management system is designed to simplify and streamline the attendance-taking process in a classroom. The system uses DynamoDB, a fast and scalable NoSQL database that provides low-latency data access. This system offers various functions that allow users to manipulate attendance records and generate reports, including adding or updating attendance records, adding or removing students from a class, and generating attendance reports for both students and classes. The proposed system is designed to increase efficiency and accuracy while reducing the administrative burden on teachers and staff.

Design:

The project design enables users to perform various operations, including adding, updating, and deleting attendance records, adding or removing students from a class, and generating attendance reports for both students and classes. The system comprises multiple functions, each with specific inputs and outputs. Users can use these functions to interact with the database and manipulate attendance data. 


Architecture:

The project is built using Python and the AWS SDK for Python, Boto3. The application connects to DynamoDB, a fully managed, NoSQL database service provided by Amazon Web Services (AWS). DynamoDB is designed to deliver fast and predictable performance by automatically distributing data across multiple partitions. It is particularly well-suited for use cases requiring low latency and high throughput, such as mobile, web, gaming, and IoT applications.
The application consists of two DynamoDB tables:
1.	ClassroomAttendance: Stores the attendance information for each student in a specific class.
2.	ClassroomRoster: Stores the roster of students for each class.

The DynamoDB table for this project will have the following structure:

| ClassID	|    Date	      |  StudentID	|   Name	     |  Attendance Status  |
------------------------------------------------------------------------------
|  0001	  |   2023-04-16	|  0001	      | John Doe 	   |   Present           |
|  0001   |   2023-04-16  |	 0002	      | Jane Smith	 |     Absent          |
|  0002	  |   2023-04-16	|  0003    	  | Alice Brown  |  	Late             |
