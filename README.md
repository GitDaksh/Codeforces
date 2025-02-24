### **Codeforces Auto-Commit 🚀**  
Automatically fetch and commit your **accepted Codeforces submissions** to this GitHub repository using **GitHub Actions**.  

![GitHub Actions Workflow](https://img.shields.io/github/actions/workflow/status/GitDaksh/Codeforces/codeforces_commit.yml?label=Auto-Commit&logo=github&style=for-the-badge)  
![Codeforces](https://img.shields.io/badge/Codeforces-Automation-blue?logo=codeforces&style=for-the-badge)  

---

## **✨ Features**
- 📡 Fetches **recent accepted submissions** from Codeforces.  
- 📂 Stores each solution in the **`submissions/`** folder, categorized by problem ID.  
- 🔄 Runs **every 15 minutes** to check for new submissions.  
- 📜 Supports **C++, Python, Java, and other languages**.  
- 🔧 Fully **automated with GitHub Actions**.  

---

## **🚀 How It Works**
1. The GitHub Actions workflow runs **every 15 minutes**.  
2. It fetches **your latest Codeforces submissions** via the **Codeforces API**.  
3. If a **new accepted solution** is found, it:  
   - **Creates a file** in `submissions/` (e.g., `1700_A.cpp`).  
   - **Commits and pushes** it automatically to GitHub.  
4. The workflow ensures **no duplicate commits** by storing a history of submissions.  

---

## **📌 Setup Instructions**
### **1️⃣ Fork This Repository**
Click **Fork** (top right) to create a copy in your GitHub account.  

### **2️⃣ Add Your GitHub Token**
1. Go to **Settings → Secrets and Variables → Actions**.  
2. Click **New Repository Secret**.  
3. Name it **`GH_TOKEN`** and paste your **GitHub Personal Access Token**.  
   - Ensure the token has **Read & Write** access to your repository.  

### **3️⃣ Edit the Workflow**
1. Open `.github/workflows/codeforces_commit.yml`.  
2. Replace **`your_codeforces_handle`** with your actual **Codeforces username**.  
3. Commit the changes.

---

## **🛠 Usage**
- **Manual Run**:  
  1. Go to the **Actions** tab in your GitHub repo.  
  2. Select **"Codeforces Auto-Commit"** workflow.  
  3. Click **"Run workflow"**.  

- **Automatic Run**:  
  - The script runs **every 15 minutes** and fetches your latest accepted submissions.  

---

## **📁 Folder Structure**
```
📂 Codeforces
 ├── 📂 submissions
 │    ├── 1700_A.cpp
 │    ├── 1805_B.py
 │    ├── 1866_C.java
 ├── submission_history.json
 ├── .github/workflows/codeforces_commit.yml
 ├── README.md
```
- **`submissions/`** → Contains all your accepted Codeforces solutions.  
- **`submission_history.json`** → Keeps track of submitted problems to avoid duplicates.  
- **`.github/workflows/codeforces_commit.yml`** → The GitHub Actions workflow file.  

---

## **🌟 Contributions**
Feel free to **fork, modify, or improve** this project! Pull requests are welcome. 🎉  

---

## **📜 License**
This project is **open-source** under the **MIT License**.  

---

🚀 **Happy Coding!** 💻🔥  

---

This **README** is structured, visually appealing, and easy to understand. Let me know if you want any modifications! 😊
