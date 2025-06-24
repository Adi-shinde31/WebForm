# 🌐 Web Form Project with EmailJS Integration

A simple, responsive web form built using **HTML, CSS, JavaScript, JQuery and EmailJS** that allows users to submit their details and receive an email confirmation — all from the frontend without a backend server!

Visit for Live Demo: `https://adi-shinde31.github.io/WebForm/`

---

## 📌 Features

- Collects user information (Name, Email, Age, DOB, Gender, Message)
- Sends a confirmation email using EmailJS
- Fully frontend (no backend or database required)
- Secure and easy to deploy on GitHub Pages or any static hosting
- Responsive design with clean UI

---

## 🛠️ Technologies Used

- HTML5
- CSS3
- JavaScript (ES6)
- [EmailJS](https://www.emailjs.com)
- jQuery (for input handling)

---

## 🚀 Installation & Setup

### 1. 📥 Clone the Repository

```bash
git clone https://github.com/your-username/webform-emailjs.git
cd webform-emailjs
```

### 2. 📄 Open the Project

You can open `index.html` directly in the browser, or host it using Live Server (VS Code Extension).

### 3. 🔐 Set Up EmailJS

#### a. Create a Free Account on [https://www.emailjs.com](https://www.emailjs.com)

#### b. Connect Your Email Service (e.g., Gmail)

- Go to **Email Services** > Add a service (like Gmail)
- Copy your **Service ID**

#### c. Create an Email Template

- Go to **Email Templates** > Create New
- Add variables like `name`, `email`, `age`, `date`, `gender`, `message`

#### d. Get Your Public Key

- Go to **Account** > **API Keys**
- Copy your **Public Key** (User ID)

---

## ⚙️ Configuration

Open `index.html` and replace the following in the `<script>` section:

```javascript
emailjs.init("YOUR_PUBLIC_KEY"); // Replace with your EmailJS public key

emailjs.send("YOUR_SERVICE_ID", "YOUR_TEMPLATE_ID", formData)
```

Replace:
- `"YOUR_PUBLIC_KEY"` → your EmailJS public key
- `"YOUR_SERVICE_ID"` → your service ID (e.g., Gmail)
- `"YOUR_TEMPLATE_ID"` → your created email template ID

---

## 📝 Email Message Template (Plain Text)

Inside your EmailJS template body:

```
========================================
🎉 Web Form Submission Confirmation
========================================

Hi {{name}}, 👋

Thank you for submitting the web form! We've received your details successfully.

Here’s what you shared with us:

📧 Email: {{email}}
🎂 Age: {{age}} y/o
📅 DOB: {{date}}
👤 Gender: {{gender}}

💬 Message:
{{message}}

Warm regards,  
Aditya Shinde  
Web Developer & Designer
```

---

## 📸 Screenshot

[![Form Screenshot](photos/output1.jpg)](https://github.com/Adi-shinde31/WebForm/blob/master/photos/Output1.jpg)

[![Email Screenshot](photos/output2.jpg)](https://github.com/Adi-shinde31/WebForm/blob/master/photos/Output2.jpg)

---

## 🧑‍💻 Author

**Aditya Shinde**  
📧 shindeaditya0258@gmail.com  
🌐 [LinkedIn](https://www.linkedin.com/in/adi-shinde31)  
🐙 [GitHub](https://github.com/adishinde31)  
💼 [Portfolio](https://adishinde31.github.io)
