Introduction to Amazon DynamoDB using AWS

This project demonstrates the implementation of a cloud-based NoSQL database system using Amazon DynamoDB on AWS. The project focuses on performing core database operations such as table creation, item insertion, querying, scanning, updating, and deleting data using the AWS Management Console.

Project Overview

Amazon DynamoDB is a fully managed NoSQL database service provided by AWS. It supports high scalability, low latency, and schema flexibility, making it suitable for modern applications such as mobile apps, web platforms, gaming systems, and IoT applications.

In this project, a Music Library Database was created to store song-related information including artist names, albums, genres, release years, and song duration.

Technologies Used
Amazon Web Services (AWS)
Amazon DynamoDB
AWS Management Console
NoSQL Database Concepts
Database Design

A DynamoDB table named Music was created with the following key structure:

Attribute Type	Name	Data Type
Partition Key	Artist	String
Sort Key	Song	String

Additional attributes used:

Album
Year
Genre
LengthSeconds

This project demonstrates DynamoDB’s schema-less nature because different items can contain different attributes.

Operations Performed
1. Creating the Table

Created a DynamoDB table named Music using:

Partition Key: Artist
Sort Key: Song
2. Inserting Records

Inserted multiple music records into the table:

Pink Floyd – Money
John Lennon – Imagine
Psy – Gangnam Style
3. Updating Data

Modified the record of Gangnam Style by updating the release year from 2011 to 2012.

4. Query Operation

Queried the table using:

Artist = Psy
Song = Gangnam Style

This retrieved the exact matching record efficiently using indexed keys.

5. Scan Operation

Performed a scan using a filter:

Year = 1971

This returned the song Imagine by John Lennon.

6. Deleting the Table

Deleted the Music table successfully after completing all operations.

Key Learning Outcomes
Understanding NoSQL databases
Working with Amazon DynamoDB
Creating and managing cloud databases
Performing CRUD operations
Understanding partition keys and sort keys
Querying and scanning data efficiently
Learning schema-less database design
Project Architecture

The project follows a serverless cloud architecture where AWS manages:

Infrastructure
Database scaling
Performance optimization
Storage management
Availability

Amazon DynamoDB acts as the core database service for storing and managing data.


Conclusion

This project provided practical exposure to AWS DynamoDB and demonstrated how NoSQL databases can efficiently manage scalable and flexible cloud-based data systems. The implementation helped in understanding real-world database operations using AWS cloud services.