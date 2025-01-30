# 📚 Student APIs – Postman Collection  

## 🚀 Overview  
This Postman collection provides a simple yet comprehensive way to interact with student records. It supports basic CRUD (Create, Read, Update, Delete) operations via **GET, POST, PUT, and DELETE** requests. The data is sourced from a `students.json` file containing records of approximately **100 students**.  

## 🌍 Base URL  
```
http://localhost:3000/students
```
## 📌 Example Student Data  
```json
{
    "id": "96",
    "name": "Sneha Singh",
    "age": 21,
    "gender": "Female",
    "email": "sneha.singh@example.com",
    "phone": "9876540492",
    "address": "Jaipur, India",
    "course": "Electronics",
    "grade": "A+"
}
```
## ⚡ Pre-Requisites  
Before running the API requests, ensure you have the following installed:  

### 1️⃣ Install [Node.js](https://nodejs.org/) and npm  
Download and install **Node.js** from the official website:  
👉 [Download Node.js](https://nodejs.org/)  

To verify installation, open **Command Prompt (cmd)** and run:  
```sh
node -v
npm -v
```
Install **json-server**
```sh
npm install -g json-server
```
Make your API up and running, use command in command line
```sh
json-server students.json
```    

## 📌 API Endpoints  

### 🔍 Get All Students  
**Method:** `GET`  
**Endpoint:**  
```
http://localhost:3000/students
```
**Description:** Fetches data of all students.  

### 🎯 Get a Single Student  
**Method:** `GET`  
**Endpoint:**  
```
http://localhost:3000/students/{id}
```
**Example:**  
```
http://localhost:3000/students/12
```
**Description:** Retrieves a specific student's details using their unique ID.  

### 📝 Create a New Student  
**Method:** `POST`  
**Endpoint:**  
```
http://localhost:3000/students
```
**Request Body (JSON Example):**  
```json
{
    "id": "101",
    "name": "Lokesh Kontey",
    "age": 32,
    "gender": "Male",
    "email": "lsingh770@gmail.com",
    "phone": "9000056804",
    "address": "Faridabad, India",
    "course": "Masters of Business Administration",
    "grade": "B+"
}
```
**Description:** Creates a new student record.  

### 🔄 Update a Student Record  
**Method:** `PUT`  
**Endpoint:**  
```
http://localhost:3000/students/{id}
```
**Example:**  
```
http://localhost:3000/students/100
```
**Request Body (JSON Example):**  
```json
{
    "name": "Lokesh Kontey",
    "age": 32,
    "gender": "Male",
    "email": "lsingh770@gmail.com",
    "phone": "9232436804",
    "address": "Faridabad, India",
    "course": "Masters of Business Administration",
    "grade": "B+"
}
```
**Description:** Updates an existing student record by specifying the ID.  

### ❌ Delete a Student Record  
**Method:** `DELETE`  
**Endpoint:**  
```
http://localhost:3000/students/{id}
```
**Example:**  
```
http://localhost:3000/students/ac82
```
**Description:** Deletes a student record using their unique ID.  


## 🛠️ How to Use  
1. **Import Collection**: Open Postman → Import the `StudentAPIs.postman_collection.json` file.  
2. **Start Local Server**: Ensure your backend API is running on `localhost:3000`.  
3. **Send Requests**: Select an API request from the collection and hit **Send**.  
4. **Check Responses**: Observe JSON responses for successful API interactions.  

## 🎯 Notes  
- Ensure the backend server is properly configured before running API calls.  
- Use appropriate **ID values** when fetching, updating, or deleting records.  
- Modify the request body in `POST` and `PUT` requests as needed.  

## 💡 Contributing  
Contributions and feedback are always welcome! 🚀  
