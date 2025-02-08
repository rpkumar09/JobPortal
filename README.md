# Job Portal
link: https://job-portal-mern-2-eqph.onrender.com/
## Overview
The **Job Portal** is a full-stack web application designed to connect job seekers with employers. It provides features such as job listings, applications, company management, user authentication, and an admin dashboard.

## Features
- User authentication (Signup/Login)
- Job seekers can browse and apply for jobs
- Employers can post and manage job listings
- Admin dashboard for managing jobs, companies, and applications
- Cloudinary integration for image uploads
- Secure API with authentication middleware

## Tech Stack
### Frontend:
- React.js (Vite)
- Tailwind CSS
- Redux Toolkit (State Management)

### Backend:
- Node.js with Express.js
- MongoDB with Mongoose ORM
- Cloudinary for image storage
- JWT for authentication

## Directory Structure
```
rpkumar09/JobPortal/
├── backend/
│   ├── controllers/        # Business logic for routes
│   ├── middlewares/        # Authentication and file handling
│   ├── models/             # Mongoose models
│   ├── routes/             # Express routes
│   ├── utils/              # Database and cloudinary configuration
│   ├── index.js            # Main backend server file
│   ├── package.json        # Backend dependencies
│   └── .gitignore          # Ignore unnecessary files
├── frontend/
│   ├── public/             # Static assets
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── hooks/          # Custom React hooks
│   │   ├── redux/          # Redux store and slices
│   │   ├── utils/          # Constants and utility functions
│   │   ├── App.jsx         # Main React component
│   │   ├── main.jsx        # Entry point for React app
│   ├── package.json        # Frontend dependencies
│   ├── tailwind.config.js  # Tailwind CSS configuration
│   └── vite.config.js      # Vite configuration
```

## Installation
### Prerequisites:
- Node.js
- MongoDB (Local or Atlas)
- Cloudinary Account (for media storage)

### Steps:
1. **Clone the repository**
   ```sh
   git clone https://github.com/rpkumar09/JobPortal.git
   cd JobPortal
   ```

2. **Backend Setup**
   ```sh
   cd backend
   npm install
   npm start
   ```
   - Create a `.env` file in the `backend` folder and add:
     ```env
     MONGO_URI=your_mongodb_uri
     JWT_SECRET=your_jwt_secret
     CLOUDINARY_CLOUD_NAME=your_cloudinary_name
     CLOUDINARY_API_KEY=your_api_key
     CLOUDINARY_API_SECRET=your_api_secret
     ```

3. **Frontend Setup**
   ```sh
   cd ../frontend
   npm install
   npm run dev
   ```

## API Endpoints
| Endpoint                     | Method | Description                      |
|------------------------------|--------|----------------------------------|
| `/api/auth/signup`           | POST   | Register a new user             |
| `/api/auth/login`            | POST   | Login and get authentication    |
| `/api/jobs`                  | GET    | Fetch all job listings          |
| `/api/jobs/:id`              | GET    | Fetch a specific job            |
| `/api/jobs`                  | POST   | Post a new job (Employer only)  |
| `/api/companies`             | GET    | Fetch all registered companies  |
| `/api/applications`          | POST   | Apply for a job                 |

## Contributing
1. Fork the repository
2. Create a new feature branch (`git checkout -b feature-name`)
3. Commit your changes (`git commit -m "Added new feature"`)
4. Push to the branch (`git push origin feature-name`)
5. Open a Pull Request

## License
This project is licensed under the MIT License.

## Contact
For any queries or suggestions, feel free to reach out via GitHub Issues.

