# Shaan Institute Website: Management Guide

## Overview

This repository contains the Shaan Institute website frontend (HTML/CSS/JS) and backend (Node.js + Express) for certificate verification and enrollment.

---

## Project Structure

- `index.html` (or your main HTML file): Frontend single-page website.
- `server.js`: Backend API server handling certificate verification and enrollment.

---

## Prerequisites

- [Node.js](https://nodejs.org/) installed (v14 or higher recommended)
- Git installed
- Text/code editor (e.g., VS Code)
- (Optional) Heroku CLI for deployment

---

## Local Development

### Frontend

1. Open `index.html` in your favorite browser directly to preview the website.
2. Edit frontend code in a text editor as needed.
3. For API calls to work locally, your backend server must be running.

### Backend

1. Open terminal in the backend folder.
2. Install dependencies:
3. Run the server:4. The backend listens on port 3000 by default.

---

## Deployment

### Backend Deployment (Heroku Example)

1. Login to Heroku CLI:2. Create a Heroku app:3. Add and commit your `Procfile` with:4. Push your code:5. Your backend will be live at `https://your-app-name.herokuapp.com`.
6. Update the frontend’s API_BASE URL to this Heroku app URL.

### Frontend Deployment

- Use platforms like GitHub Pages, Netlify, or Vercel for hosting static files.
- Upload your `index.html` (and assets if any) following their instructions.

---

## Managing Content

- Edit the frontend HTML file to update text, styles, or layout.
- Backend logic changes require updating `server.js`.

---

## Managing Backend Data

- Current certificate IDs are stored in-memory in `server.js`.
- For production, integrate with a database (MongoDB, SQL, etc.) for persistence.
- Enrollment data can be saved similarly or emailed via a mailing service.

---

## Recommended Workflow

1. Edit code locally.
2. Test frontend and backend on localhost.
3. Commit changes to Git.
4. Deploy backend and frontend to hosting providers.
5. Monitor logs and user feedback regularly.

---

## Useful Commands
undefined
---

## Support

Feel free to contact the developer or open issues in the repository for assistance.

---

## License

MIT License (or your license here)

---

*Managed and maintained by Shaan Institute*
