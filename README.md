# Vscode-project-
Link to web vscode project  run command
Here's a step-by-step guide to upload your HTML and C project to GitHub and run it using Termux:

---

### 1. **Upload Project to GitHub**
1. **Prepare Your Files:**
   - Make sure your project directory contains all necessary files for both the HTML and C parts.
   - Add a `README.md` file to explain the project.

2. **Create a GitHub Repository:**
   - Go to [GitHub](https://github.com/wwwstawberrycom/Vscode-project-) and log in.
   - Click on **"New Repository"**.
   - Enter a name, description, and choose **Public** or **Private**.
   - Do **not** add a README file, `.gitignore`, or license (we'll do this locally).

3. **Upload Files Locally:**
   Open a terminal and run the following commands:
   ```bash
   cd https://github.com/wwwstawberrycom/Vscode-project-
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add https://github.com/wwwstawberrycom/Vscode-project-
   git push -u origin main
   ```

---

### 2. **Clone Project in Termux**
1. **Install Git in Termux:**
   Open Termux and run:
   ```bash
   pkg update
   pkg upgrade
   pkg install git
   ```

2. **Clone the Repository:**
   ```bash
   git clone https://github.com/wwwstawberrycom/Vscode-project-.git
   cd vscode_dg
   ```

---

### 3. **Run the Project in Termux**
1. **For C Files:**
   - Install GCC:
     ```bash
     pkg install clang
     ```
   - Compile and run the C program:
     ```bash
     clang vscode_web.c -o output
     ./output
     ```

2. **For HTML Files:**
   - Install a text-based web browser like `w3m`:
     ```bash
     pkg install w3m
     ```
   - Run the HTML file:
     ```bash
     w3m index.html
     ```

---

### 4. **Optional: Install a Local Web Server**
To test the HTML project in a browser:
   ```bash
   pkg install python
   python -m http.server
   ```
   - Access the project locally by opening `http://localhost:8000` in a browser.

This process will let you work with your HTML and C projects directly on GitHub and Termux.
