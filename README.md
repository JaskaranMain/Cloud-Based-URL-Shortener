# Cloud-Based-URL-Shortener
Cloud-Based URL Shortener (Java + AWS)

🚀 Overview

This is a Cloud-Based URL Shortener built using Java, AWS Lambda, DynamoDB, and API Gateway. It converts long URLs into short ones (similar to Bit.ly) and retrieves the original URL when accessed. This project demonstrates AWS cloud integration with minimal Spring Boot usage, making it a great addition to your resume for Cloud/Software Engineering roles.

🛠️ Tech Stack

Java (Core Java, Collections, Hashing)

Spring Boot (Minimal - for REST APIs)

AWS Lambda (Serverless processing)

DynamoDB (NoSQL database for storage)

API Gateway (Exposes REST APIs)

AWS SDK for Java (To interact with AWS services)

🎯 Features

✅ Shortens long URLs into unique short URLs
✅ Stores short URLs in AWS DynamoDB
✅ Retrieves original URLs when accessed
✅ Uses AWS Lambda for serverless execution
✅ API Gateway to expose APIs securely
✅ Spring Boot for REST API handling
✅ Secure API calls with JWT authentication (Optional)

📁 Project Structure

/url-shortener
   ├── src/main/java/com/urlshortener
   │   ├── controller  # Handles API requests
   │   ├── service     # URL shortening logic
   │   ├── repository  # DynamoDB integration
   │   ├── model       # Data models
   │   ├── UrlShortenerApplication.java  # Main application file
   ├── pom.xml  # Dependencies
   ├── README.md  # Project documentation

⚙️ How It Works

1️⃣ User sends a long URL via REST API (POST /shorten)</br>
2️⃣ A hashing function generates a short URL</br>
3️⃣ The short URL is stored in AWS DynamoDB</br>
4️⃣ User accesses the short URL (GET /{shortURL}), and the original URL is retrieved</br>
5️⃣ AWS Lambda processes the request without needing a server</br>
6️⃣ API Gateway acts as the entry point for API calls</br>

🛠️ AWS Services Used
</br>
AWS Lambda → Serverless execution

DynamoDB → NoSQL database

API Gateway → Exposes REST APIs

IAM Roles → Secure access management

🔥 Future Improvements

Implement Redis caching for faster lookups

Add custom short URLs instead of generated ones

Track URL analytics using AWS CloudWatch

🎯 Contributing

Feel free to fork this repo, open issues, or submit pull requests! 🚀


⭐ If you found this project useful, give it a star on GitHub! ⭐
