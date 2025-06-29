# JobWebApp
Job Application Management System
A simple web-based job posting and management application built with Spring Boot and Thymeleaf.
🚀 Features

Add New Jobs: Post job listings with title, description, experience requirements, and tech stack
View All Jobs: Browse all posted job listings in a clean, card-based layout
Responsive Design: Bootstrap-styled interface that works on all devices
Form Validation: Ensures proper job data entry
RESTful Architecture: Clean separation between controller, service, and data layers

🛠️ Tech Stack

Backend: Spring Boot 3.x
Frontend: Thymeleaf, HTML5, CSS3
Styling: Bootstrap 5
Build Tool: Maven
Java Version: 17+

📋 Prerequisites
Before running this application, make sure you have:

Java 17 or higher installed
Maven 3.6+ installed
IDE (IntelliJ IDEA, Eclipse, or VS Code)

🚦 Getting Started
1. Clone the Repository
bashgit clone <your-repository-url>
cd JobApp
2. Build the Project
bashmvn clean install
3. Run the Application
bashmvn spring-boot:run
Or run directly from your IDE by executing the main class:
javaJobAppApplication.java
4. Access the Application
Open your browser and navigate to:
http://localhost:8080
📁 Project Structure
src/
├── main/
│   ├── java/
│   │   └── com/leon/JobApp/
│   │       ├── JobAppApplication.java     # Main Spring Boot class
│   │       ├── JobController.java         # Web controller
│   │       ├── model/
│   │       │   └── JobPost.java          # Job entity model
│   │       └── service/
│   │           └── JobService.java       # Business logic layer
│   └── resources/
│       ├── static/
│       │   └── css/
│       │       └── style.css            # Custom styles
│       └── templates/
│           ├── addjob.html              # Add job form
│           ├── viewalljobs.html         # Job listings page
│           └── success.html             # Success confirmation
└── pom.xml                              # Maven dependencies
🔗 Available Endpoints
MethodEndpointDescriptionGET/Home pageGET/addjobDisplay add job formPOST/handleFormProcess new job submissionGET/viewalljobsDisplay all job listings
💼 Job Model
Each job posting contains:

Post Profile: Job title/position
Post Description: Detailed job description
Required Experience: Years of experience needed
Tech Stack: List of required technologies

🎨 UI Features

Dark Theme: Modern dark cards with white text
Responsive Grid: 2-column layout that adapts to screen size
Bootstrap Components: Professional styling with Bootstrap 5
Form Validation: Client and server-side validation

🔧 Configuration
Application Properties
properties# Server configuration
server.port=8080

# Thymeleaf configuration
spring.thymeleaf.cache=false
🐛 Troubleshooting
Common Issues:

CSS not loading (404 error)

Ensure style.css is in src/main/resources/static/css/
Check template reference: <link href="/css/style.css" rel="stylesheet">


NullPointerException in controller

Verify @Service annotation on JobService
Ensure proper dependency injection with @Autowired or constructor injection


Template not found

Verify templates are in src/main/resources/templates/
Check return value matches template name



Debug Mode
Add to application.properties:
propertieslogging.level.org.springframework.web=DEBUG
logging.level.org.thymeleaf=DEBUG
📝 Usage Examples
Adding a New Job

Navigate to /addjob
Fill in the job details:

Job Title: "Senior Java Developer"
Description: "Looking for experienced Java developer..."
Experience: "5"
Tech Stack: "Java, Spring Boot, MySQL"


Click "Submit"
Success page confirms job was added

Viewing All Jobs

Navigate to /viewalljobs
Browse job cards showing all posted positions
Each card displays title, description, experience, and tech stack

🚀 Future Enhancements

 Database integration (H2, MySQL, PostgreSQL)
 Job search and filtering
 User authentication and authorization
 Job application functionality
 Admin panel for job management
 REST API endpoints
 Email notifications

🤝 Contributing

Fork the repository
Create a feature branch: git checkout -b feature-name
Commit changes: git commit -am 'Add feature'
Push to branch: git push origin feature-name
Submit a pull request

👨‍💻 Author
Created by George Kumi Acheampong
📞 Support
If you encounter any issues or have questions:

Open an issue on GitHub
Email: kwameleon21@gmail.com
