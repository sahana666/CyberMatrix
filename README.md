# 🛡️ LandShield — Smart Land Protection & Property Risk Analysis

**LandShield** is a web application designed to help users investigate property details, analyze potential land-related risks, review property evidence, and stay informed about possible land protection concerns.

The platform brings property investigation, risk assessment, evidence analysis, and alerts together in one dashboard.

## ✨ Features

- **🔐 User Authentication** — Login and account registration interface.
- **📊 Interactive Dashboard** — Centralized view of property investigation and land protection features.
- **🔎 Property Search** — Search and investigate property records.
- **⚠️ Property Risk Assessment** — Analyze property risk information and identify potential concerns.
- **📄 Document Analysis** — Upload documents for property-related analysis.
- **🗂️ Evidence Review** — Organize and display:
  - Survey Evidence
  - Ownership Evidence
  - Mortgage / Encumbrance Evidence
- **🔔 Alerts & Notifications** — Review property-related alerts and risk information.
- **🛡️ Land Protection** — Tools to support land protection and property investigation workflows.
- **📅 Land Visit Reminders** — Keep track of planned property visits.
- **🔗 Backend API Integration** — Connect the frontend to a backend API using an environment variable.
- **📚 Property Records** — The project currently includes 279 property records.

## 🧰 Tech Stack

| Technology   | Purpose                              |
| ------------ | ------------------------------------ |
| React        | User interface                       |
| Vite         | Development server and build tooling |
| JavaScript   | Application logic                    |
| CSS          | Styling and responsive UI            |
| REST API     | Frontend and backend communication   |
| Git & GitHub | Version control and collaboration    |

> Add any additional technologies used by your backend, such as FastAPI, Flask, Node.js, or a database, once you confirm the actual stack.

## 📁 Project Structure

The frontend is organized around the following key files:

```text
LandShield/
├── public/
├── src/
│   ├── App.jsx
│   ├── index.css
│   ├── main.jsx
│   └── ...
├── .env.example
├── .gitignore
├── index.html
├── package.json
├── package-lock.json
├── vite.config.js
└── README.md
```

_Your actual folder structure may contain additional pages, components, assets, and backend files._

## ⚙️ Getting Started

### Prerequisites

Install the following before running the project:

- [Node.js](https://nodejs.org/) — preferably a current LTS version.
- npm — included with Node.js.
- Git — for cloning and version control.
- A running backend API, if using backend-connected features.

### 1. Clone the repository

Replace `YOUR_USERNAME` with your GitHub username.

```bash
git clone https://github.com/YOUR_USERNAME/LandShield.git
```

Navigate to the project folder:

```bash
cd LandShield
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Create a `.env` file in the project root.

```env
VITE_API_URL=http://127.0.0.1:8000/api
```

The frontend uses `VITE_API_URL` as the backend API base URL. If this variable is not configured, the application defaults to the URL shown above.

**Important:** Make sure the backend is running at the configured address before testing API-connected features.

Do not put passwords, API secrets, or private credentials in frontend environment variables. Variables prefixed with `VITE_` can be exposed to browser users.

### 4. Start the development server

```bash
npm run dev
```

Open the local URL printed in your terminal, usually:

```text
http://localhost:5173
```

### 5. Build for production

```bash
npm run build
```

To preview the production build locally:

```bash
npm run preview
```

## 🔌 Backend Configuration

LandShield uses a configurable API base URL for backend communication.

Example:

```javascript
const API_BASE_URL =
  import.meta.env.VITE_API_URL || "http://127.0.0.1:8000/api";
```

Set `VITE_API_URL` to your deployed backend URL when running the frontend in production.

If the frontend and backend run on different origins, configure the backend's CORS policy to allow requests from the frontend origin.

Backend-specific installation instructions should be added here once the backend framework, dependencies, and startup command are confirmed.

## 🧭 How to Use LandShield

1. Start the backend API, if required.
2. Start the React development server.
3. Open the application in your browser.
4. Sign in or use the available registration flow.
5. Explore the dashboard and property search features.
6. Select a property to review its available information and risk assessment.
7. Review survey, ownership, and mortgage or encumbrance evidence when available.
8. Upload supported property documents for analysis.
9. Review alerts and use land visit reminders to support follow-up.

_Available features and results depend on the configured backend, data sources, and application setup._

## 🔒 Security & Privacy

- Never commit `.env` files containing secrets.
- Keep authentication credentials and private keys out of the frontend source code.
- Validate uploaded documents on the backend.
- Enforce authentication and authorization on protected API endpoints.
- Treat property risk assessments as decision-support information, not as a substitute for official land records or professional legal advice.

## 🚀 Future Improvements

Potential enhancements include:

- Integration with verified government land-record sources.
- Improved property ownership and encumbrance verification.
- Interactive maps and property boundary visualization.
- Advanced risk scoring and explainable risk indicators.
- More comprehensive document extraction and evidence matching.
- User-specific notifications and investigation history.
- Automated testing and deployment workflows.

## 🤝 Contributing

Contributions and suggestions are welcome.

1. Fork the repository.
2. Create a feature branch:

   ```bash
   git checkout -b feature/your-feature
   ```

3. Commit your changes:

   ```bash
   git commit -m "Add your feature"
   ```

4. Push your branch:

   ```bash
   git push origin feature/your-feature
   ```

5. Open a pull request.

## ⚠️ Disclaimer

LandShield is intended to support property research and land protection workflows. Risk scores and document analysis should be independently verified against authoritative records. The application does not itself establish legal ownership or guarantee that a property is free from disputes or encumbrances.

## 👨‍💻 Author

**Project:** LandShield  
**Category:** Property Technology · Land Protection · Risk Analysis

---

⭐ If you find this project useful, consider giving the repository a star!
