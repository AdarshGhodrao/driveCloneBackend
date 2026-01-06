<div align="center">

<h1>📂 DriveClone Backend</h1>

<p><strong>A backend service for a cloud file storage application (DriveClone)</strong></p>

<p>
  Spring Boot · Java · MongoDB · JWT · OAuth2 · Cloudinary
</p>

</div>

<hr/>

<h2>🌟 Overview</h2>

<p>
The <strong>DriveClone Backend</strong> is a RESTful API built with Spring Boot that provides backend support for a Google Drive–style application.  
It handles authentication, file and folder management, uploads to cloud storage, user profiles, and secure API access for frontend clients.
</p>

<hr/>

<h2>✨ Features</h2>

<ul>
  <li>User authentication and authorization using JWT</li>
  <li>OAuth2-based login integration</li>
  <li>File upload and download handling</li>
  <li>Folder and file organization</li>
  <li>Cloud-based media storage integration</li>
  <li>Role-based access and permissions</li>
  <li>Email support via SMTP</li>
</ul>

<hr/>

<h2>🛠️ Tech Stack</h2>

<table border="1" cellpadding="8" cellspacing="0">
  <tr>
    <th>Component</th>
    <th>Technology</th>
  </tr>
  <tr>
    <td>Framework</td>
    <td>Spring Boot</td>
  </tr>
  <tr>
    <td>Language</td>
    <td>Java</td>
  </tr>
  <tr>
    <td>Database</td>
    <td>MongoDB</td>
  </tr>
  <tr>
    <td>Security</td>
    <td>Spring Security, JWT, OAuth2</td>
  </tr>
  <tr>
    <td>File Storage</td>
    <td>Cloud Storage Service</td>
  </tr>
  <tr>
    <td>Build Tool</td>
    <td>Maven</td>
  </tr>
</table>

<hr/>

<h2>🚀 Getting Started</h2>

<h3>Clone the Repository</h3>
<pre>
git clone &lt;repository-url&gt;
cd DriveCloneBackend
</pre>

<h3>Install Dependencies</h3>
<pre>
mvn clean install
</pre>

<h3>Run Locally</h3>
<pre>
mvn spring-boot:run
</pre>

Your backend will start on:
<code>http://localhost:8080</code>

<hr/>

<h2>🔐 Environment Variables (Required)</h2>

<p>Create <code>src/main/resources/application.properties</code> (ignored by Git) and define the following:</p>

<pre>
# Application
spring.application.name=DriveCloneBackend

# MongoDB
spring.data.mongodb.uri=
spring.data.mongodb.database=DriveClone

# Cloud Storage
cloudinary.cloud-name=
cloudinary.api-key=
cloudinary.api-secret=

# Email SMTP
spring.mail.host=smtp.gmail.com
spring.mail.port=587
spring.mail.username=
spring.mail.password=

# OAuth2
spring.security.oauth2.client.registration.google.client-id=
spring.security.oauth2.client.registration.google.client-secret=

# JWT
jwt.secret=
</pre>

<p><strong>Note:</strong> Never commit sensitive credentials. Always use environment variables or secure configuration files.</p>

<hr/>

<h2>🌐 API Endpoints</h2>

<h3>Authentication</h3>
<pre>
POST /api/auth/login
POST /api/auth/register
GET  /api/auth/oauth
POST /api/auth/logout
</pre>

<h3>User Management</h3>
<pre>
GET    /api/user/profile
PUT    /api/user/update
DELETE /api/user/delete
</pre>

<h3>Folder & File Operations</h3>
<pre>
GET    /api/files/all
POST   /api/files/upload
GET    /api/files/download/{id}
DELETE /api/files/delete/{id}
</pre>

<hr/>

<h2>📁 Project Structure</h2>

<pre>
DriveCloneBackend/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/example/driveclone/
│   │   │       ├── config/
│   │   │       ├── controller/
│   │   │       ├── dto/
│   │   │       ├── entity/
│   │   │       ├── repository/
│   │   │       ├── service/
│   │   │       └── DriveCloneBackendApplication.java
│   ├── resources/
│   │   └── application.properties.example
├── pom.xml
└── README.md
</pre>

<hr/>

<h2>🤝 Contributing</h2>

<ul>
  <li>Fork the repository</li>
  <li>Create a feature branch</li>
  <li>Write clean and tested code</li>
  <li>Submit a Pull Request</li>
</ul>

<hr/>

<h2>💬 Support</h2>

<ul>
  <li>Open an issue for bug reports or feature requests</li>
  <li>Contact the maintainer for collaboration</li>
</ul>

<hr/>

<div align="center">
  <p><strong>⭐ If you find this project helpful, please give it a star</strong></p>
  <p>Made by <strong>Adarsh Ghodrao</strong></p>
</div>

<h1>driveCloneBackend</h1>

