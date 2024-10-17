# MongoDB-shell-commands

## Prerequisites

Before you begin, ensure you have:

* Installed MongoDB on your machine.
* Set up mongosh, the MongoDB shell.

## How to Start MongoDB Shell (mongosh)

1. Launch MongoDB server: Before using mongosh, make sure your MongoDB server is running. You can do this by typing:

``` bash
mongod
```
2. Start MongoDB Shell: In a new terminal window, use the following command to start mongosh:

```bash

mongosh
```
This will connect to the default localhost server.


## Creating the Database and Collections

Once you're in the mongosh shell, you can proceed with the following commands:

1. Create or switch to the Codetribe database:

```bash
use Codetribe
```

2. Create a collection named Facilitators and insert a document:

```bash
db.Facilitators.insertOne({
    Name: "John Doe",
    Location: "Cape Town",
    Course: "Web Development"
})
```

3. Create a collection named Trainees and insert a document:

``` bash
db.Trainees.insertOne({
    Name: "Jane Smith",
    Location: "Johannesburg",
    Facilitator: "John Doe"
})
```

4. Create a collection named Projects and insert a document:

``` bash
db.Projects.insertOne({
    Name: "E-commerce Website",
    Course: "Web Development",
    Lesson: "MongoDB Basics"
})
```


## Viewing the Inserted Documents

You can verify that your documents have been inserted correctly by using the following command for each collection:

* View all documents in Facilitators:

``` bash
db.Facilitators.find().pretty()
```

* View all documents in Trainees:

```bash
db.Trainees.find().pretty()
```

* View all documents in Projects:

```bash
db.Projects.find().pretty()
```


## Additional MongoDB Commands

* Show all databases:

``` bash
show dbs
```

* Show collections in the current database:

```bash
show collections
```

* Delete a specific document:

```bash
db.Facilitators.deleteOne({ Name: "John Doe" })
```

* Drop a collection:

```bash
db.Projects.drop()
```
With these commands, you'll be able to create and manage the Codetribe database effectively.

## This is an example of  how the server should look when started
![sever](https://github.com/user-attachments/assets/849eb002-7c73-4ff0-9b3f-3283dd2d2615)

## This is an example of shell started
![shell](https://github.com/user-attachments/assets/adb43bb2-518e-4e5d-85ce-303868cb2f42)

