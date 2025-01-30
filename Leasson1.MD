# 🔹 Lesson 1: Understanding How Websites Work

Before hacking anything, you must understand how websites function. Let's start with basic web concepts.

---

## 1️⃣ The Basics of Websites
A website is made of multiple components:

- **Front-end (Client-side)**: This is what you see (HTML, CSS, JavaScript).
- **Back-end (Server-side)**: This is what powers the website (PHP, Python, Node.js).
- **Database**: Stores website data (MySQL, PostgreSQL, MongoDB).

---

## 2️⃣ How Websites Communicate (HTTP & HTTPS)
Websites use the **HTTP** protocol to communicate with users. Think of it as a conversation between your browser and a web server.

## 🔹 HTTP Response Example (What the server replies with):

HTTP/1.1 200 OK
Content-Type: text/html
<html>
  <body>Hello, World!</body>
</html>

🔹 **HTTPS** is a secure version of HTTP using encryption (**SSL/TLS**).

---

## 3️⃣ Understanding URLs (Uniform Resource Locator)

A URL is the **address** of a webpage. Example:

https://example.com:443/login.php?id=1

### Breaking it down:
- `https` → **Protocol**
- `example.com` → **Domain name**
- `443` → **Port number** (default for HTTPS)
- `/login.php` → **Webpage** (endpoint)
- `?id=1` → **Query parameter** (used in SQL Injection!)

---

## 4️⃣ Understanding Cookies & Sessions

Websites use **cookies** and **sessions** to remember users.

- **Cookies** are stored in your browser and sent with every request.
- **Sessions** are stored on the server.

### Example:
Cookie: PHPSESSID=123456789abcdef

### Why do hackers care?
- **Session hijacking**: Stealing cookies to log in as someone else.
- **Session fixation**: Forcing a user to use a specific session ID.

---

## 🔹 Hands-On Task #1: Inspect Web Traffic

### 🛠️ Task: Use Browser DevTools

1. Open **Google Chrome**.
2. Press **F12** or **Ctrl + Shift + I** to open Developer Tools.
3. Click on the **"Network"** tab.
4. Reload the page (**F5**) and check the **HTTP requests**.
5. Look at the **Headers tab**. Identify:
   - **Host**
   - **Cookies**
   - **User-Agent**
   - **Response Status Code** (e.g., 200 OK, 404 Not Found)

👉 **Take a screenshot** of what you find and share your observations!
