# Voting App – DevOps Pipeline Tutorial

A simple fullstack web app to practice CI/CD pipeline with GitHub Actions and deployment to Render.

✅ Click here for [LIVE DEMO](https://voting-app-devops-tutorial.onrender.com)

![Screenshot](https://github.com/alfhisa/voting-app-devops-tutorial/raw/main/demo.png)

## Features

- Vote between Python, JavaScript, and Go
- Realtime results with live update
- Minimal and responsive UI
- GitHub Actions CI
- Easy deploy to [Render](https://render.com)

## How to Run Locally

```bash
git clone https://github.com/your-username/voting-app-devops-tutorial.git
cd voting-app-devops-tutorial
npm install
npm start
```

Visit `http://localhost:3000` in your browser.

## CI Pipeline with GitHub Actions

The CI workflow is defined at:

```bash
.github/workflows/ci.yml
```

### What It Does:
- Installs dependencies
- Runs build script
- Optionally runs tests (you can extend it)
- Ensures build passes before deployment

To enable:
1. Push your project to GitHub.
2. GitHub Actions will automatically trigger the CI on every `push` or `pull_request`.

---

## Deployment to Render (Free Hosting)

You can deploy this fullstack app in **minutes**.

### Steps:

1. Go to [https://render.com](https://render.com) and log in with GitHub
2. Click **"New Web Service"**
3. Connect to your GitHub repo:  
   `voting-app-devops-tutorial`
4. Set these values:
   - **Environment**: `Node`
   - **Build Command**: `npm install`
   - **Start Command**: `npm start`
   - **Root Directory**: Leave empty (if `package.json` is in root)
5. Click **Create Web Service**
6. Wait for Render to build and deploy your app

Done! Your app will be live with a public URL like:  
`https://voting-app-devops.onrender.com`

---

## Credits

By [@alfhisa](https://github.com/alfhisa) for teaching purposes.
