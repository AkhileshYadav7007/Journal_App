# 📝 Journal App

A full-featured **Journal App** built using **Java**, **Spring Boot**, **MongoDB Atlas**, **Redis**, and **Kafka**, with an intuitive AWT-based user interface. This app allows users to create, read, update, and delete journal entries in a secure, real-time, and scalable way. 

---

## 🚀 Features

- 🖊️ Create, Read, Update, Delete (CRUD) journal entries
- ☁️ MongoDB Atlas for cloud-based storage
- 🧠 Redis for in-memory caching to boost performance
- 📢 Kafka for real-time data streaming and activity logging
- 📋 AWT GUI for interactive journal management
- 🔒 Secure backend using Spring Boot
- ☁️ AWS for cloud deployment
- 📆 Auto-timestamp entries
- 🔍 Search functionality with instant response
- ⚡ Fast, scalable, and lightweight

---

## 🛠️ Tech Stack

| Layer         | Technology               |
|---------------|--------------------------|
| Language      | Java                     |
| Backend       | Spring Boot              |
| Database      | MongoDB Atlas            |
| Caching       | Redis                    |
| Messaging     | Apache Kafka             |
| UI            | AWT (Abstract Window Toolkit) |
| Cloud         | AWS (EC2, S3, IAM)       |
| Build Tool    | Maven / Gradle           |
| Dev Tools     | IntelliJ IDEA, Git, Postman |

---

## 🧩 Architecture Overview

```text
+-----------+      +------------+      +-------------+
|   AWT UI  +----->+ Spring Boot+----->+ MongoDB Atlas|
+-----------+      +------------+      +-------------+
                       |
                       +--> Redis (for fast reads)
                       |
                       +--> Kafka (for async logging/events)
📸 Screenshots
(Add screenshots of the GUI, Kafka logs, Redis CLI output, etc.)

🔧 Setup Instructions
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/yourusername/Journal-App.git
cd Journal-App
2. MongoDB Atlas Setup
Create a cluster at MongoDB Atlas

Replace the URI in application.properties:

properties
Copy
Edit
spring.data.mongodb.uri=mongodb+srv://<user>:<password>@cluster0.mongodb.net/journalDB
3. Redis Setup
Install Redis locally or use Redis Cloud

properties
Copy
Edit
spring.redis.host=localhost
spring.redis.port=6379
4. Kafka Setup
Install and start Zookeeper & Kafka:

bash
Copy
Edit
# Start Zookeeper
bin/zookeeper-server-start.sh config/zookeeper.properties

# Start Kafka Broker
bin/kafka-server-start.sh config/server.properties
Update Kafka config in application.properties:

properties
Copy
Edit
spring.kafka.bootstrap-servers=localhost:9092
spring.kafka.consumer.group-id=journal-group
5. Run the Application
Maven:
bash
Copy
Edit
./mvnw spring-boot:run
IntelliJ:
Run JournalAppApplication.java

🖥️ GUI Interface (AWT)
Clean form to create/edit entries

Entry list window to view, update, or delete

Real-time feedback via Kafka logging

📬 Kafka Use Case
Logs every journal action (create, update, delete)

Topics: journal-events

Can be extended to integrate with analytics or email alerts

🚀 Redis Use Case
Caches frequent reads (like recent journal entries)

Reduces DB calls, improving speed

TTL set for automatic cache eviction

📂 Project Structure
swift
Copy
Edit
Journal-App/
│
├── src/main/java/com/example/journalapp/
│   ├── controller/
│   ├── model/
│   ├── repository/
│   ├── service/
│   ├── config/         # Redis and Kafka config
│   ├── util/
│   └── JournalAppApplication.java
│
├── src/main/resources/
│   ├── application.properties
│   └── static/
│
├── README.md
└── pom.xml / build.gradle
🧪 Testing
✅ Manual UI testing (AWT)

✅ API testing via Postman

✅ Kafka consumer log verification

✅ Redis CLI or monitoring tool for cache hit/miss

👨‍💻 Author
Akhilesh Yadav
📍 Ayodhya, Uttar Pradesh
📫 akhileshyadavji7007@gmail.com
