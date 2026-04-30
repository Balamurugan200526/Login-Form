<div align="center">

```
██╗      ██████╗  ██████╗ ██╗███╗   ██╗    ███████╗ ██████╗ ██████╗ ███╗   ███╗
██║     ██╔═══██╗██╔════╝ ██║████╗  ██║    ██╔════╝██╔═══██╗██╔══██╗████╗ ████║
██║     ██║   ██║██║  ███╗██║██╔██╗ ██║    █████╗  ██║   ██║██████╔╝██╔████╔██║
██║     ██║   ██║██║   ██║██║██║╚██╗██║    ██╔══╝  ██║   ██║██╔══██╗██║╚██╔╝██║
███████╗╚██████╔╝╚██████╔╝██║██║ ╚████║    ██║     ╚██████╔╝██║  ██║██║ ╚═╝ ██║
╚══════╝ ╚═════╝  ╚═════╝ ╚═╝╚═╝  ╚═══╝    ╚═╝      ╚═════╝ ╚═╝  ╚═╝╚═╝     ╚═╝
```

# 🔐 User Registration Form

### *A sleek, client-side registration experience — no backend required.*

<br>

[![Live Demo](https://img.shields.io/badge/🌐%20Live%20Demo-Visit%20Now-28a745?style=for-the-badge&logoColor=white)](https://balamurugan200526.github.io/Login-Form/)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222222?style=for-the-badge&logo=github&logoColor=white)](https://pages.github.com/)

<br>

---

</div>

## ✨ Overview

> A beautifully crafted **User Registration Form** built with pure HTML, CSS, and JavaScript — no frameworks, no fuss. Data is stored locally in the browser using `localStorage`, making it perfect for demos, prototypes, and learning projects.

<div align="center">

```
┌──────────────────────────────────┐
│        User Registration         │
│  ┌──────────────────────────┐   │
│  │  👤  Enter Username       │   │
│  └──────────────────────────┘   │
│  ┌──────────────────────────┐   │
│  │  🔒  Enter Password       │   │
│  └──────────────────────────┘   │
│  ⚠️  Data stored locally (demo) │
│  ┌──────────────────────────┐   │
│  │        Register          │   │
│  └──────────────────────────┘   │
└──────────────────────────────────┘
```

</div>

---

## 🚀 Features

| Feature | Description |
|---|---|
| 🎨 **Gradient Background** | Eye-catching blue-to-green gradient |
| ✅ **Form Validation** | Real-time alerts for empty fields |
| 💾 **LocalStorage** | Saves user data directly in the browser |
| 🔁 **Auto Reload** | Page refreshes after successful registration |
| 📱 **Responsive** | Centered layout that works on all screen sizes |
| ⚡ **Zero Dependencies** | Pure HTML + CSS + Vanilla JS |

---

## 🛠️ Tech Stack

```
📁 Project
├── 🌐  HTML5        →  Structure & Semantics
├── 🎨  CSS3         →  Gradient, Flexbox, Animations
└── ⚙️  JavaScript   →  Validation + LocalStorage API
```

---

## 📂 Project Structure

```
📦 Login-Form/
 ┣ 📄 index.html       ← All-in-one: markup, styles & scripts
 ┗ 📄 README.md        ← You're reading it!
```

---

## ⚙️ How It Works

```mermaid
graph TD
    A[👤 User fills form] --> B{Fields empty?}
    B -- Yes --> C[🚨 Alert shown]
    B -- No --> D[💾 Save to localStorage]
    D --> E[🎉 Success Alert]
    E --> F[🔁 Page Reloads]
```

**Step-by-step flow:**

1. User enters a **username** and **password**
2. JavaScript **validates** both fields are non-empty
3. User data is **saved to `localStorage`** as a JSON array
4. A **success alert** is displayed with the username
5. The page **automatically reloads** for a fresh start

---

## 💻 Getting Started

### Option 1 — View Live 🌐
Click the badge below and you're done!

[![Live Demo](https://img.shields.io/badge/🌐%20Open%20Live%20Demo-28a745?style=for-the-badge)](https://balamurugan200526.github.io/Login-Form/)

---

### Option 2 — Run Locally 🖥️

```bash
# 1. Clone the repository
git clone https://github.com/balamurugan200526/Login-Form.git

# 2. Navigate to project folder
cd Login-Form

# 3. Open in browser
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

> 💡 No build steps. No installs. Just open and go!

---

## 🔍 Code Highlights

### 🔒 Validation Logic
```javascript
function validateForm() {
    let username = document.getElementById("username").value.trim();
    let password = document.getElementById("password").value.trim();

    if (username === "") { alert("Please enter a username."); return false; }
    if (password === "") { alert("Please enter a password."); return false; }

    // Store to localStorage
    let users = JSON.parse(localStorage.getItem("users")) || [];
    users.push({ username, password });
    localStorage.setItem("users", JSON.stringify(users));

    alert("Registration successful for " + username + "!");
    location.reload();
    return false;
}
```

### 🎨 Gradient Background
```css
background: linear-gradient(to right, blue, green);
```

---

## 📸 Preview

```
<img width="1878" height="903" alt="image" src="https://github.com/user-attachments/assets/f99c51a1-5f1e-4679-b297-4abbb2f52222" />

```

---

## 🗺️ Roadmap

- [x] Basic registration form
- [x] LocalStorage integration
- [x] Form validation
- [ ] 🔐 Password strength indicator
- [ ] 👁️ Show/Hide password toggle
- [ ] 🌙 Dark mode support
- [ ] 📤 Backend integration (Node.js / Firebase)
- [ ] 🔑 Login page with credential verification

---

## 🤝 Contributing

Contributions are welcome! Here's how:

```bash
# 1. Fork the project
# 2. Create your feature branch
git checkout -b feature/AmazingFeature

# 3. Commit your changes
git commit -m "Add some AmazingFeature"

# 4. Push to the branch
git push origin feature/AmazingFeature

# 5. Open a Pull Request
```

---

## 📜 License

```
MIT License — Free to use, modify, and distribute.
```

---

## 👨‍💻 Author

<div align="center">

**Balamurugan**

[![GitHub](https://img.shields.io/badge/GitHub-balamurugan200526-181717?style=for-the-badge&logo=github)](https://github.com/balamurugan200526)
[![Live Project](https://img.shields.io/badge/Live%20Project-Login%20Form-28a745?style=for-the-badge&logo=googlechrome&logoColor=white)](https://balamurugan200526.github.io/Login-Form/)

---

*⭐ If you found this project helpful, please give it a star! It means a lot.*

```
Made with ❤️ and pure JavaScript — no frameworks harmed in the making of this form.
```

</div>
