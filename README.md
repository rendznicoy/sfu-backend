# Express + Multer Backend Server

Backend server for handling single file uploads using **Express.js**, **Multer**, and **EJS**.

## Description
This backend accepts file uploads from the React frontend, stores them on the server, and provides routes to view or delete files. It uses EJS for templating and Tailwind CSS for a simple UI.

## Features
- Upload a single file from a client or an HTML form.
- Delete files by filename.
- View all uploaded files in JSON or via an EJS-rendered page.
- Static route to serve uploaded files.

## Technologies
- **Express.js** – Web framework.
- **Multer** – Middleware for handling `multipart/form-data` uploads.
- **EJS** – View engine for rendering HTML pages.
- **Tailwind CSS** – For styling.

## Installation & Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/rendznicoy/sfu-backend.git
   
2. Navigate to the project folder:
   ```bash
    cd sfu-backend
   
3. Install dependencies:
   ```bash
   npm install express multer ejs
   
4. Start the server:
   ```bash
   node server.js

5. Open your browser:
   ```arduino
   http://localhost:3000 or http://localhost:5000
   
## API Endpoints
Method	Route	Description
- GET	/	Render index.html page
- POST	/upload	Upload a single file
- DELETE	/delete/:name	Delete a file by filename
- GET	/view	View all uploaded files (JSON)
- GET	/uploads/:file	Serve uploaded file

## Usage
1. Upload: Use the /upload route from your React frontend or directly from the rendered form.

2. Delete: Send a DELETE request to /delete/:fileName.

3. View Files: Visit /view to list files or /uploads/{filename} to access a file.

4. Download Files
