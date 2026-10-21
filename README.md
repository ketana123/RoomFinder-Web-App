# Room Finder

Room Finder is an academic team project intended to help users find room/hostel rental listings. The project uses Java Servlets, HTML/CSS, Maven, and MySQL.

> **Academic team project:** Update the team member names and contributions below before publishing.

## Features represented in the source
- User registration and login
- Room-owner registration and login
- Admin login with OTP email flow
- Room/owner information pages and dashboards
- MySQL database access through DAO classes

## Technology Stack
- Java 8
- Java Servlets (`javax.servlet`)
- Maven
- MySQL
- HTML and CSS
- JavaMail for OTP email

## Project Structure
```text
RoomFinder/
├── pom.xml
├── README.md
├── .gitignore
├── .env.example
└── src/
    ├── com/model/              # Model classes
    ├── dao_classes/            # Database access
    ├── servlet_connecction/    # Servlet controllers
    └── main/webapp/
        ├── WEB-INF/web.xml
        ├── *.html
        └── style.css
```

## Requirements
- JDK 8 or compatible JDK
- Maven
- MySQL Server
- A Java servlet container such as Apache Tomcat 9 (the source uses `javax.servlet`)
- A MySQL database and tables matching the queries used in the DAO classes

## Configuration
The source no longer contains the database password or Gmail app password. Configure these environment variables in your local run environment:

- `ROOMFINDER_DB_URL` — for example, `jdbc:mysql://localhost:3306/project`
- `ROOMFINDER_DB_USER` — your local MySQL username
- `ROOMFINDER_DB_PASSWORD` — your local MySQL password
- `ROOMFINDER_ADMIN_EMAIL` — email address allowed to request admin OTP
- `ROOMFINDER_MAIL_FROM` — sender email address
- `ROOMFINDER_MAIL_PASSWORD` — email provider app password

See `.env.example` for names only. Do not put real passwords or app passwords in GitHub.

## Build
From the project root, run:

```bash
mvn clean package
```

This creates a WAR file under `target/` when the project dependencies and local setup are correct. Deploy the WAR to a compatible servlet container such as Tomcat 9.

## Database setup
The original ZIP did not include a database export or schema script. Create the MySQL database and tables required by the SQL queries in `src/dao_classes/` before running the application. Do not upload real user data.

## Team Members
- **Member 1:** [Name] — [Contribution]
- **Member 2:** [Name] — [Contribution]
- **Member 3:** [Name] — [Contribution]

## Project Information
- **Course:** MCA
- **Semester:** 2
- **Project Type:** Academic team mini project

## Notes
This repository is a cleaned source package based on the provided project ZIP. The application has not been executed or end-to-end tested as part of packaging. Review the source, database setup, and team credits before publishing.
