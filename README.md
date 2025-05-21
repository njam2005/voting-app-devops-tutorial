# Voting App – DevOps Pipeline Tutorial

A simple fullstack web app designed for students to **learn and practice CI/CD pipeline** using GitHub Actions and deployment to [Render](https://render.com).

🚀 [LIVE DEMO](https://voting-app-devops-tutorial.onrender.com) – deployed from this repository  

![Screenshot](https://github.com/alfhisa/voting-app-devops-tutorial/raw/main/demo.png)

---

## What You'll Learn

- How to fork a repo and deploy your own web app
- How CI/CD works using GitHub Actions
- How to deploy to free hosting with Render
- How Docker, pipeline automation, and deployment relate to DevOps

---

## Features

- Simple voting app
- Real-time results display
- Minimal and responsive UI
- GitHub Actions CI pipeline
- One-click deploy to Render (Node.js hosting)

---

## Instructions for Students

### 1. **Fork This Repository**

Click the **"Fork"** button on the top-right of this GitHub repo. This will create a copy of the repo under your own GitHub account.

---

### 2. **Run Locally (Optional)**

```bash
git clone https://github.com/your-username/voting-app-devops-tutorial.git
cd voting-app-devops-tutorial
npm install
npm start
```

Then open `http://localhost:3000` in your browser.

---

### 3. **Deploy to Render (Free Hosting)**

#### Steps:

1. Go to [https://render.com](https://render.com) and log in with your GitHub.
2. Click **"New Web Service"**.
3. Choose **your forked repo** (e.g. `voting-app-devops-tutorial`).
4. Use the following settings:
   - **Environment**: `Node`
   - **Build Command**: `npm install`
   - **Start Command**: `npm start`
   - **Root Directory**: *(leave empty)*
5. Click **"Create Web Service"**.
6. Wait for Render to build and deploy your app.

Once done, your voting app will be available at a public URL like:
```
https://your-app-name.onrender.com
```

---

## CI Pipeline with GitHub Actions

GitHub Actions workflow file is located at:

```
.github/workflows/ci.yml
```

It will:
- Run `npm install` to install dependencies
- Optionally run tests (can be extended)
- Ensure build success before allowing deployment

The pipeline is automatically triggered on:
- `push` to any branch
- Pull requests

---

## Credits

This tutorial is created by [@alfhisa](https://github.com/alfhisa) for educational use in DevOps and Software Engineering courses.
