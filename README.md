# Cloud-Based-URL-Shortener
Cloud-Based URL Shortener (Java + AWS)

<h2>🚀 Overview</h2>

This is a Cloud-Based URL Shortener built using Java, AWS Lambda, DynamoDB, and API Gateway. It converts long URLs into short ones (similar to Bit.ly) and retrieves the original URL when accessed. This project demonstrates AWS cloud integration with minimal Spring Boot usage, making it a great addition to your resume for Cloud/Software Engineering roles.

<h2>🛠️ Tech Stack</h2>

Java (Core Java, Collections, Hashing)
Spring Boot (Minimal - for REST APIs)
AWS Lambda (Serverless processing)
DynamoDB (NoSQL database for storage)
API Gateway (Exposes REST APIs)
AWS SDK for Java (To interact with AWS services)

<h2>🎯 Features</h2>

✅ Shortens long URLs into unique short URLs</br>
✅ Stores short URLs in AWS DynamoDB</br>
✅ Retrieves original URLs when accessed</br>
✅ Uses AWS Lambda for serverless execution</br>
✅ API Gateway to expose APIs securely</br>
✅ Spring Boot for REST API handling</br>
✅ Secure API calls with JWT authentication (Optional)</br>

<h2>📁 Project Structure</h2>

/url-shortener </br>
   ├── src/main/java/com/urlshortener </br>
   │   ├── controller  # Handles API requests </br>
   │   ├── service     # URL shortening logic </br>
   │   ├── repository  # DynamoDB integration </br>
   │   ├── model       # Data models </br>
   │   ├── UrlShortenerApplication.java  # Main application file </br>
   ├── pom.xml  # Dependencies </br>
   ├── README.md  # Project documentation </br>

<h2>⚙️ How It Works</h2>

1️⃣ User sends a long URL via REST API (POST /shorten)</br>
2️⃣ A hashing function generates a short URL</br>
3️⃣ The short URL is stored in AWS DynamoDB</br>
4️⃣ User accesses the short URL (GET /{shortURL}), and the original URL is retrieved</br>
5️⃣ AWS Lambda processes the request without needing a server</br>
6️⃣ API Gateway acts as the entry point for API calls</br>

<h2>🛠️ AWS Services Used</h2>
</br>
AWS Lambda → Serverless execution
DynamoDB → NoSQL database
API Gateway → Exposes REST APIs
IAM Roles → Secure access management
</br>
<h2>🔥 Future Improvements</h2>
</br>
Implement Redis caching for faster lookups
</br>
Add custom short URLs instead of generated ones
</br>
Track URL analytics using AWS CloudWatch
</br>
<h2>🎯 Contributing</h2>
</br>
Feel free to fork this repo, open issues, or submit pull requests! 🚀
<hr>
</br>
⭐ If you found this project useful, give it a star on GitHub! ⭐
