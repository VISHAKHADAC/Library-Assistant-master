# WebService

This project contains a web service for **user registration**, featuring:

- **Frontend**: React
- **Backend**: Spring Boot

---

## 🚀 Installation

Follow these steps to set up and run the application locally.

1. **Clone the repository:**
   git clone <project-url>

2. **Navigate to the project directory:**
   cd <project-directory>

3. **Start the React frontend:**
   cd frontend
   npm install
   npm start

4. **Start the Spring Boot backend:**
   cd ..
   mvn spring-boot:run

5. **Access the application:**
   Visit http://localhost:5173 in your browser.

---

## 🧑‍💻 Usage

WebService provides a simple interface for user registration.

The React frontend allows users to enter:

- Username
- Email address
- Password

The Spring Boot backend processes and saves the data.

---

## 📡 API Endpoints

### ✅ Create User Registration

- URL: /api/v1/users
- Method: POST
- Description: Create a new user registration.

🔸 Parameters

Name     | Type   | Required | Description
---------|--------|----------|-------------------------
username | string | Yes      | User's username
email    | string | Yes      | User's email address
password | string | Yes      | User's password

🔸 Example Request

POST /api/v1/users HTTP/1.1
Content-Type: application/json

{
  "username": "user",
  "email": "user@example.com",
  "password": "password123"
}

✅ Successful Response

{
  "status": "success",
  "data": {
    "id": 1,
    "username": "user",
    "email": "user@example.com"
  }
}

❌ Error Response

{
  "status": "error",
  "message": "Username already taken."
}

---

## ✨ Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

---

## 📝 License
This project is licensed under the MIT License.
