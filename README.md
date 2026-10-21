# html-to-jsp-conversion
# Student Information System | Java Servlet & JSP

## 📌 Project Overview
The **Student Information System** is a simple Java web application developed using Java Servlets and JSP (JavaServer Pages). It allows users to enter student details through a registration form and displays the submitted information on a result page.

This project demonstrates the basic working of Java web technologies, form handling, and request forwarding.

## ✨ Features
- Student registration form
- Input fields for Name, Email, Course, and Age
- Form submission using the HTTP POST method
- Request handling using Java Servlet
- Display of submitted details using JSP Expression Language (EL)
- Simple and beginner-friendly web application

## 🛠️ Technologies Used
- **Java** – Application logic
- **Java Servlets** – Handling form submissions
- **JSP (JavaServer Pages)** – Web pages and result display
- **HTML** – Registration form structure
- **Maven** – Project build and dependency management
- **Apache Tomcat 11** – Web application server
- **Jakarta Servlet API** – Servlet functionality

## 📂 Project Structure

```text
servlet/
├── src/
│   └── main/
│       ├── java/
│       │   └── com/
│       │       └── servlet/
│       │           └── HelloServlet.java
│       └── webapp/
│           ├── student.jsp
│           └── result.jsp
├── pom.xml
└── README.md
```

*Note: The structure above represents the typical Maven layout. Your actual folder structure may differ.*

## ⚙️ How It Works
1. The user opens the student registration page (`student.jsp`).
2. The user enters their name, email, course, and age.
3. The form submits the data to the `/hello` servlet using the POST method.
4. `HelloServlet.java` retrieves the submitted data.
5. The servlet stores the values as request attributes.
6. The request is forwarded to `result.jsp`.
7. The result page displays the submitted student details.

## 🚀 How to Run the Project

### Prerequisites
- Java JDK
- Apache Maven
- Apache Tomcat 11
- Visual Studio Code or another Java IDE

### Steps
1. Clone or download this repository.
2. Open the project folder in Visual Studio Code.
3. Ensure that `pom.xml` contains the required Jakarta Servlet API dependency.
4. Build the project using:

   ```bash
   mvn clean package
   ```

5. Deploy the generated WAR file from the `target` folder to Apache Tomcat 11.
6. Start the Tomcat server.
7. Open the application in your browser:

   ```text
   http://localhost:8080/servlet/student.jsp
   ```

   Replace `servlet` with your actual deployed application context path if it differs.

## 📸 Application Workflow
**Registration Page → HelloServlet → Registration Result Page**

## 🎯 Learning Outcomes
- Understanding Java Servlet lifecycle basics
- Working with HTTP GET and POST concepts
- Retrieving form data using `request.getParameter()`
- Passing data using request attributes
- Forwarding requests from Servlet to JSP
- Using JSP Expression Language to display data

## 🔮 Future Improvements
- Connect the application to a MySQL database
- Add server-side input validation
- Store student records permanently
- Improve the user interface using CSS and Bootstrap
- Add student search, update, and delete functionality


