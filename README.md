# 🌍 LONDON LTD

A modern and responsive corporate website for **LONDON LTD**, featuring a clean frontend and a Node.js + Express backend for handling contact form submissions.

---

## ✨ Features

- Modern and responsive design
- Smooth user experience
- Contact form with backend integration
- REST API built with Node.js and Express
- Stores and retrieves contact submissions
- Health check endpoint
- Mobile, tablet, and desktop support

---

## 🛠️ Technologies Used

### Frontend
- HTML5
- CSS3
- JavaScript
- Vite

### Backend
- Node.js
- TypeScript
- Express
- CORS

---

## 📂 Project Structure

```text
.
├── src/
│   ├── server.ts          # Express backend
│   ├── main.ts
│   └── components/
├── public/
├── index.html
├── package.json
├── tsconfig.json
└── README.md
```

---

# 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/london-ltd.git
```

Move into the project folder:

```bash
cd london-ltd
```

Install dependencies:

```bash
npm install
```

---

# ⚙️ Backend Setup

The project includes a Node.js + Express server located in:

```text
src/server.ts
```

### Install required backend packages

```bash
npm install express cors @types/express @types/cors
```

If TypeScript execution is not installed:

```bash
npm install -D ts-node typescript
```

---

# ▶️ Running the Backend

Start the Express server:

```bash
npx ts-node src/server.ts
```

By default, the API runs on:

```text
http://localhost:3001
```

---

# 📡 API Endpoints

### Health Check

```http
GET /api/health
```

Example:

```http
GET http://localhost:3001/api/health
```

Response:

```json
{
  "status": "ok"
}
```

---

### Submit Contact Form

```http
POST /api/contact
```

Example body:

```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "message": "Hello!"
}
```

---

### Get All Contact Submissions

```http
GET /api/contact
```

Returns all saved form submissions.

---

# 🌐 Environment Variables

The frontend uses:

```env
VITE_API_URL=http://localhost:3001
```

Create a `.env` file in the project root:

```env
VITE_API_URL=http://localhost:3001
```

---

# 🖥️ Running the Frontend

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

The website will usually be available at:

```text
http://localhost:5173
```

---

# 🚀 Running Everything

Terminal 1:

```bash
npm run dev
```

Terminal 2:

```bash
npx ts-node src/server.ts
```

Frontend:

```text
http://localhost:5173
```

Backend:

```text
http://localhost:3001
```

---

# 📱 Responsive Design

Optimized for:

- 💻 Desktop
- 📱 Mobile
- 📲 Tablet

---

# 📄 License

This project is licensed under the MIT License.

---

Made with ❤️ for **LONDON LTD**