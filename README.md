# 🏮 Lantern – Lost & Found Registry

A modern **serverless Lost & Found web application** built on **AWS Cloud** that helps users report, browse, edit, and manage lost and found items in real time.

The application provides a clean user interface and uses AWS services to store images, manage item records, and expose REST APIs without managing servers.

---

# 📸 Project Preview

![Lantern Banner](./assets/banner.png)

> *(Replace with your project screenshot after uploading one.)*

---

# ✨ Features

- 📌 Report Lost Items
- 📌 Report Found Items
- 📷 Upload Item Images
- 🔍 Search Items
- 🎯 Filter by Lost / Found
- ✏️ Edit Existing Records
- 🗑 Delete Records
- 📱 Fully Responsive UI
- ⚡ Fast Serverless Backend
- ☁️ AWS Cloud Hosted
- 🚀 Automatic Deployment using GitHub Actions

---

# 🏗 Architecture

```
                User
                  │
                  ▼
        Static Website (EC2 + Nginx)
                  │
                  ▼
          API Gateway (REST API)
                  │
                  ▼
              AWS Lambda
                  │
         ┌────────┴─────────┐
         ▼                  ▼
     DynamoDB             Amazon S3
(Item Metadata)       (Item Images)
```

---

# ☁️ AWS Services Used

| Service | Purpose |
|----------|----------|
| EC2 | Host Frontend |
| Nginx | Web Server |
| API Gateway | REST APIs |
| Lambda | Backend Logic |
| DynamoDB | Store Item Details |
| Amazon S3 | Store Uploaded Images |
| IAM | Permissions |
| CloudWatch | Logging |
| GitHub Actions | CI/CD Deployment |

---

# 📂 Project Structure

```
Lantern-The-Lost-Found-Website/

│
├── .github/
│   └── workflows/
│       └── main.yml
│
├── images/
│
├── index.html
├── style.css
├── script.js
│
├── README.md
│
└── backend/
    ├── lambda_function.py
    └── requirements.txt
```

---

# 🚀 Deployment Architecture

```
Developer

    │

Git Push

    │

GitHub Repository

    │

GitHub Actions

    │

SSH

    │

AWS EC2

    │

Git Pull

    │

Nginx Reload

    │

Updated Website
```

---

# ⚙️ Installation

## Clone Repository

```bash
git clone https://github.com/Jagruti345/Lantern-The-Lost-Found-Website.git
```

```
cd Lantern-The-Lost-Found-Website
```

---

## Frontend

Open

```
index.html
```

or host using Nginx.

---

## Backend

Deploy Lambda function using

- Python 3.x
- API Gateway
- DynamoDB
- Amazon S3

Update the API URL inside

```
script.js
```

```javascript
const API = "https://YOUR_API_GATEWAY_URL";
```

---

# 📡 API Endpoints

## Get Items

```
GET /items
```

Returns all lost and found items.

---

## Add Item

```
POST /items
```

Request

```json
{
    "item":"Wallet",
    "location":"Library",
    "concernPerson":"John",
    "contactNumber":"9876543210",
    "status":"lost",
    "image":"Base64 Image"
}
```

---

## Update Item

```
PUT /items/{itemId}
```

---

## Delete Item

```
DELETE /items/{itemId}
```

---

# 📷 Screenshots

## Home Page

*(Add Screenshot)*

---

## Report Item

*(Add Screenshot)*

---

## Registry

*(Add Screenshot)*

---

# 🔒 Security

- IAM Least Privilege
- API Gateway Validation
- Secure Image Storage in S3
- No Database Credentials Stored in Frontend

---

# 📈 Future Improvements

- User Authentication
- Admin Dashboard
- Email Notifications
- QR Code Item Tracking
- AI Image Matching
- Rekognition Integration
- SMS Notifications
- Dark Mode
- Mobile App

---

# 🧪 Technologies Used

### Frontend

- HTML5
- CSS3
- JavaScript

### Backend

- Python
- AWS Lambda

### Database

- Amazon DynamoDB

### Storage

- Amazon S3

### Deployment

- GitHub Actions
- EC2
- Nginx

---

# 👩‍💻 Author

**Jagruti Patil**

GitHub

https://github.com/Jagruti345

---

# ⭐ Support

If you like this project, consider giving it a ⭐ on GitHub.

---

# 📜 License

This project is licensed under the MIT License.
