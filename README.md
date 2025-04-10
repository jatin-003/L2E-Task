# Student Enrollment Form

This is a modern, minimal, and fully functional **Student Enrollment Form** web application built using **HTML, CSS, JavaScript, jQuery**, and the **Login2Explore JPDB API**. The form allows users to **create** and **update** student records securely with logical validations and a sleek UI.

---

## Features

- **Auto Roll No Check**  
  Automatically checks if a student with the entered Roll No already exists in the database and enables the appropriate mode (Save or Update).

- **Minimalist Responsive UI**  
  Clean, mobile-friendly layout using Bootstrap 4 with custom enhancements.

- **Field Validations**  
  All fields are required. Logical validation ensures Enrollment Date is after Birth Date.

- **Create and Update Support**  
  Insert new student records or update existing ones with ease using PUT and UPDATE requests.

- **Auto Enable/Disable Fields**  
  Fields are enabled or disabled based on Roll No existence and operation mode.

---

## Technologies Used

- **Frontend**: HTML5, CSS3, Bootstrap 4, JavaScript, jQuery  
- **Backend/Database**: JPDB (Login2Explore JSON PowerDB)

---

## Benefits of Using JsonPowerDB

JsonPowerDB (JPDB) is a high-performance, lightweight, and secure JSON-based database engine that offers several advantages, especially for frontend-integrated projects like this one:

- **Schema-Free Design**  
  Flexible data structure allows quick iterations and dynamic form processing without altering backend schemas.

- **Integrated REST API**  
  No need for separate backend logic or server setup — interact directly with the database via secure API calls.

- **Fast and Lightweight**  
  Optimized for low-latency operations with fast read/write speeds and minimal overhead.

- **Built-in Indexing**  
  Key-based access is efficient and direct, enabling quick data retrieval for operations like Roll No lookup.

- **Ideal for Frontend Projects**  
  Enables full-stack functionality within the frontend using JavaScript — perfect for rapid prototypes or student-level projects.

- **Secure and Controlled Access**  
  Use of a connection token ensures controlled and authenticated access to the database.

- **Hosted Service**  
  No deployment headaches — JPDB is cloud-hosted and ready to use out of the box.

---
## Folder Structure

```
student-enrollment/
│
├── index.html         # Main UI with integrated logic
└── README.md          # Project documentation
```

---

## Getting Started

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/student-enrollment.git
   cd student-enrollment
   ```

2. **Open `index.html` in Browser**  
   You can open the file directly in a browser or use a local web server for better development experience.

---

## API Configuration

Make sure you are using a valid **Login2Explore JPDB API token** and database/relationship names:

```javascript
const jpdbBaseURL = "http://api.login2explore.com:5577";
const dbName = "SCHOOL-DB";
const relName = "STUDENT-TABLE";
const connToken = "your-connection-token-here";
```

> Replace `connToken` with your own secure token obtained from [Login2Explore](http://login2explore.com/).

---

## Logical Validations

- No field can be left empty.
- Enrollment date must be later than the birth date.
- Duplicate Roll Numbers are not allowed when saving a new record.
- Update mode only works for existing Roll Numbers.

---

## Screenshots

# Submitting / Updating Data
![image](https://github.com/user-attachments/assets/c3e3257d-b0db-459f-ba60-c9f92cb66d78)

# Verification in the Console
![image](https://github.com/user-attachments/assets/1faa18eb-962b-4941-8bc2-858201b57048)


---

## License

This project is released under the **MIT License** — feel free to use and adapt it as needed.

