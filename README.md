# Student and Group CRUD JSP Project

This project is a Java web application for managing students and groups using JSP (JavaServer Pages) technology. It provides CRUD (Create, Read, Update, Delete) functionality for both students and groups, with features including secure admin pages, login functionality with remember me option, cascading deletion of students when a group is deleted, and password encryption using bcrypt.

## Technologies Used

- **Java Backend**: Utilizes Java for server-side logic and business operations.
- **Hibernate JPA**: Object-relational mapping framework for working with PostgreSQL database.
- **PostgreSQL**: Open-source relational database management system.
- **JSP (JavaServer Pages)**: Dynamic web pages technology for displaying HTML content with Java code.
- **Bootstrap**: Front-end framework for creating responsive and visually appealing web pages.
- **Servlets**: Handles requests and responses between the client and server.
- **Tomcat**: Servlet container that hosts the Java web application.
- **Cookies**: Utilized for implementing the remember me functionality.
- **bcrypt**: Library for password hashing and encryption.

## Features

- **CRUD Operations**: Allows creating, reading, updating, and deleting both students and groups.
- **Search Engine**: The main page includes a search engine where users can be searched with the similarity of first name or last name.
- **Secure Admin Pages**: Access to admin pages is restricted to authenticated users only.
- **Login Page**: Provides a login page for user authentication.
- **Remember Me Checkbox**: Users can choose to stay logged in even after the session is disconnected by checking the "Remember Me" checkbox.
- **Cookie-Based Session Management**: Saves a cookie on the user's device to maintain their login status across sessions if the "Remember Me" option is selected.
- **Cascading Deletion**: When a group is deleted, all associated students are automatically removed from the PostgreSQL database to maintain data integrity.
- **Password Encryption**: User passwords are encrypted using bcrypt before storing them in the database. During login, the password entered by the user is hashed and compared with the hashed password retrieved from the database for authentication.
- **Error Notification**: If the user enters incorrect credentials during login, the login page displays a notification informing them that either the email or password is wrong and prompts them to try again.

  <img src="screenshots/login%20page.jpg" alt="Project Screenshot" width="300">
  <img src="screenshots/main%20page.jpg" alt="Project Screenshot" width="300">
  <img src="screenshots/admin%20page.jpg" alt="Project Screenshot" width="300">


## Installation and Setup

1. Clone the repository to your local machine:

git clone https://github.com/yourusername/student-group-crud-jsp.git


2. Import the project into your preferred IDE (Eclipse, IntelliJ, etc.).
3. Set up the PostgreSQL database and configure the connection details in the project's configuration files.
4. Deploy the application to a servlet container such as Apache Tomcat.
5. Access the application through your web browser.

## Usage

1. Navigate to the login page and enter your credentials.
2. Optionally, check the "Remember Me" checkbox to stay logged in across sessions.
3. Access the admin pages to perform CRUD operations on students and groups.
4. Log out when finished using the application.

## Contributing

Contributions are welcome! Please feel free to submit issues, feature requests, or pull requests to help improve this project.
