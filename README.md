# 📝 Journal App

A full-featured **Journal App** built using **Java**, **Spring Boot**, **MongoDB Atlas**, and **AWS**, with an intuitive user interface developed using **AWT (Abstract Window Toolkit)**. The app allows users to securely create, read, update, and delete journal entries. Whether you're logging daily reflections or keeping track of tasks, this app has you covered!

---

## 🚀 Features

- 🖊️ Create, Read, Update, Delete (CRUD) journal entries
- ☁️ Cloud-based data storage using MongoDB Atlas
- 📋 Intuitive GUI built using AWT
- 🔒 Secure backend with Spring Boot
- ☁️ Hosted/Integrated with AWS Services (EC2/S3)
- 📆 Timestamped entries
- 🔍 Search functionality
- 💡 Lightweight and easy to deploy

---

## 🛠️ Tech Stack

| Layer        | Technology             |
|--------------|------------------------|
| Language     | Java                   |
| Backend      | Spring Boot            |
| Database     | MongoDB Atlas          |
| UI           | AWT (Java GUI)         |
| Cloud        | AWS (EC2, S3, etc.)    |
| Dev Tools    | IntelliJ IDEA, Postman, Git |
| Build Tool   | Maven/Gradle           |

---

## 📸 Screenshots

> (Include screenshots here if possible)
> - Dashboard View  
> - Create Entry Window  
> - Entry List View

---

## 🔧 Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/Journal-App.git
cd Journal-App
2. Configure MongoDB Atlas
Set up a MongoDB cluster on MongoDB Atlas

Whitelist your IP

Create a database and collection

Copy your connection string and update it in application.properties:

properties
Copy
Edit
spring.data.mongodb.uri=mongodb+srv://<username>:<password>@cluster0.mongodb.net/journalDB?retryWrites=true&w=majority
3. Build & Run the Project
Using Maven:
bash
Copy
Edit
./mvnw spring-boot:run
Or Using IDE:
Open in IntelliJ or Eclipse

Run the main class: com.yourpackage.JournalAppApplication

🖥️ GUI Interface (AWT)
The GUI is built using Java’s AWT library

Provides a clean form for journal entry creation

Shows list of saved entries and allows edits/deletes

☁️ AWS Integration
EC2: Host backend services

S3: (Optional) Store user images or attached files

IAM: Manage credentials and policies

Secrets Manager: Securely store DB credentials (optional)

📂 Project Structure
swift
Copy
Edit
Journal-App/
│
├── src/
│   ├── main/
│   │   ├── java/com/example/journalapp/
│   │   │   ├── controller/
│   │   │   ├── model/
│   │   │   ├── repository/
│   │   │   ├── service/
│   │   │   └── JournalAppApplication.java
│   │   └── resources/
│   │       ├── application.properties
│   │       └── static/
│
├── README.md
└── pom.xml / build.gradle
🧪 Testing
Use Postman or Swagger UI (if integrated) to test REST APIs

Manual GUI testing for AWT components

✍️ Author
Akhilesh Yadav
📍 Ayodhya, Uttar Pradesh
📫 akhileshyadavji7007@gmail.com
