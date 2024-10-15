
# CodeTribe MongoDB Project

This project demonstrates how to use MongoDB to create a database and collections, insert documents, and retrieve data using the MongoDB shell (`mongosh`).

## Prerequisites

Ensure MongoDB is installed and running on your local machine. You can download it from [here](https://www.mongodb.com/try/download/community).

## How to Start the MongoDB Shell (Mongosh)

1. **Start MongoDB:**
   - Open PowerShell and start the MongoDB shell by typing:
     ```bash
     mongosh
     ```

   This command connects to the local MongoDB instance.

2. **Connected to:**
   ```
   mongodb://127.0.0.1:27017/?directConnection=true&serverSelectionTimeoutMS=2000&appName=mongosh+2.3.2
   ```

## Database Creation

### Switch to the Database

To create and switch to the `CodeTribe` database, use:
```bash
use CodeTribe
```
This command switches to the database. If the database does not exist, it will be created once you insert a collection.

## Collection and Document Creation

Below are the MongoDB commands used to create collections and insert documents.

### 1. Facilitators Collection

To insert a document into the `Facilitators` collection:
```bash
db.Facilitators.insertOne({
    Name: "Mahlatse",
    Location: "Soweto",
    Course: "MERN Stack Development"
})
```

### 2. Trainees Collection

To insert a document into the `Trainees` collection:
```bash
db.Trainees.insertOne({
    Name: "Xolile",
    Location: "Soweto",
    Facilitator: "Mahlatse"
})
```

### 3. Projects Collection

To insert a document into the `Projects` collection:
```bash
db.Projects.insertOne({
    Name: "MongoDB with Mongosh",
    Course: "MERN Stack Development",
    Lesson: "MongoDB Lesson 2"
})
```

## Querying Data

You can retrieve documents from each collection using the following commands.

### 1. Facilitators Collection

To retrieve all documents from the `Facilitators` collection:
```bash
db.Facilitators.find({})
```

### 2. Trainees Collection

To retrieve all documents from the `Trainees` collection:
```bash
db.Trainees.find({})
```

### 3. Projects Collection

To retrieve all documents from the `Projects` collection:
```bash
db.Projects.find({})
```

## Summary

- **Database:** `CodeTribe`
- **Collections:** `Facilitators`, `Trainees`, `Projects`
- **Fields:**
  - Facilitators: `Name`, `Location`, `Course`
  - Trainees: `Name`, `Location`, `Facilitator`
  - Projects: `Name`, `Course`, `Lesson`

This project shows basic MongoDB operations, including creating a database, inserting data into collections, and retrieving documents using the MongoDB shell.

## Author

**Xoli Nxiweni**  
- Email: [xolinxiweni@gmail.com](mailto:xolinxiweni@gmail.com)  
- GitHub: [Xoli-Nxiweni/MongoDB-L2](https://github.com/Xoli-Nxiweni/MongoDB-L2.git)

For more information, refer to the [MongoDB Documentation](https://docs.mongodb.com/).

---