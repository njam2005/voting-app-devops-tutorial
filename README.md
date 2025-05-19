# Voting App – DevOps Pipeline Tutorial

A simple fullstack web app to practice CI/CD pipeline with GitHub Actions and deployment to Render.

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

## GitHub Actions CI

Pipeline defined in `.github/workflows/ci.yml`

## Deployment

Deploy this app to Render:
- New Web Service → Connect repo
- Build Command: `npm install`
- Start Command: `npm start`
- Environment: Node.js

## Credits

By [@alfhisa](https://github.com/alfhisa) for teaching purposes.
