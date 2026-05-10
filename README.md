# 🎵 Introduction to Amazon DynamoDB using AWS

This project demonstrates the implementation of a cloud-based NoSQL database system using **Amazon DynamoDB** on **Amazon Web Services (AWS)**. The project focuses on performing core database operations such as table creation, item insertion, querying, scanning, updating, and deleting records using the AWS Management Console.

---

# 📌 Project Overview

Amazon DynamoDB is a fully managed NoSQL database service provided by AWS. It offers:

- High scalability
- Low latency
- Flexible schema design
- Automatic scaling
- Serverless architecture

These features make DynamoDB suitable for modern applications such as:

- Mobile applications
- Web applications
- Gaming systems
- IoT platforms
- Real-time systems

In this project, a **Music Library Database** was created to store and manage song-related information including artists, albums, genres, release years, and song duration.

---

# 🛠 Technologies Used

- Amazon Web Services (AWS)
- Amazon DynamoDB
- AWS Management Console
- NoSQL Database Concepts

---

# 🗂 Database Design

A DynamoDB table named **Music** was created using the following primary key structure:

| Attribute Type | Attribute Name | Data Type |
|----------------|----------------|-----------|
| Partition Key  | Artist         | String    |
| Sort Key       | Song           | String    |

## Additional Attributes

- Album
- Year
- Genre
- LengthSeconds

The project demonstrates DynamoDB’s **schema-less architecture**, where different items can contain different attributes without requiring a fixed schema.

---

# ⚙ Operations Performed

## 1️⃣ Creating the Table

Created a DynamoDB table named **Music** using:

- Partition Key → `Artist`
- Sort Key → `Song`

---

## 2️⃣ Inserting Records

Inserted multiple music records into the table:

| Artist | Song |
|--------|------|
| Pink Floyd | Money |
| John Lennon | Imagine |
| Psy | Gangnam Style |

---

## 3️⃣ Updating Data

Updated the existing item:

- Modified the release year of **Gangnam Style**
- Changed the value from **2011 → 2012**

---

## 4️⃣ Query Operation

Queried the table using indexed keys:

```text
Artist = Psy
Song = Gangnam Style
```

This retrieved the exact matching record efficiently.

---

## 5️⃣ Scan Operation

Performed a scan operation using a filter condition:

```text
Year = 1971
```

The scan operation returned:

- Imagine by John Lennon

---

## 6️⃣ Deleting the Table

Deleted the **Music** table successfully after completing all operations.

---

# 📚 Key Learning Outcomes

Through this project, the following concepts were learned:

- Understanding NoSQL databases
- Working with Amazon DynamoDB
- Creating and managing cloud databases
- Performing CRUD operations
- Understanding partition and sort keys
- Querying and scanning data efficiently
- Learning schema-less database design
- Understanding serverless cloud architecture

---

# ☁ Project Architecture

The project follows a **serverless cloud architecture** where AWS automatically manages:

- Infrastructure
- Database scaling
- Performance optimization
- Storage management
- Availability

Amazon DynamoDB acts as the core database service for storing and managing all music-related data.

---

# 📄 Project Report

The detailed project report is available in the repository:

```text
report/DynamoDB-project.pdf
```

---

# ✅ Conclusion

This project provided practical exposure to **Amazon DynamoDB** and demonstrated how NoSQL databases can efficiently manage scalable and flexible cloud-based data systems.

The implementation helped in understanding:

- Real-world database operations
- AWS cloud services
- Serverless database management
- Efficient data retrieval techniques

Overall, the project strengthened practical knowledge of cloud computing and NoSQL database technologies using AWS.

---

# 🔖 Tags

`AWS` `DynamoDB` `NoSQL` `Cloud Computing` `Database Management` `Serverless` `AWS Project`
