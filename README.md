# QORE - Complete Full Stack Recruitment Application

QORE is a comprehensive recruitment platform featuring both backend API and frontend interface for managing the entire recruitment process. This repository contains the complete application with all files including environment configurations.

## 🚀 Project Structure

```
qorefullapplication/
├── QORE Backend/           # Node.js/Express backend API
│   ├── src/               # Source code
│   ├── docs/              # API documentation
│   ├── scripts/           # Database scripts
│   ├── migrations/        # Database migrations
│   ├── seeders/          # Database seeders
│   ├── .env              # Environment variables
│   ├── package.json      # Backend dependencies
│   └── index.js          # Main server file
├── QORE Frontend/         # React/TypeScript frontend
│   ├── src/              # Source code
│   ├── public/           # Static assets
│   ├── server/           # Backend server for file uploads
│   ├── components/       # React components
│   ├── pages/           # Application pages
│   ├── .env             # Environment variables
│   ├── package.json     # Frontend dependencies
│   └── vite.config.ts   # Vite configuration
└── README.md            # This file
```

## ✨ Features

### Backend Features
- 🔐 User authentication and authorization (JWT)
- 🛡️ Role-based access control (RBAC)
- 👥 Employee management system
- 💼 Job posting and management
- 📅 Interview scheduling
- 📄 Resume parsing and analysis
- 📧 Email notifications
- 📱 SMS notifications
- 🏢 Multi-branch support
- 📊 Reports and analytics

### Frontend Features
- ⚛️ Modern React application with TypeScript
- 🎨 Responsive UI with Tailwind CSS
- 🧩 Reusable components with Radix UI
- 🔑 Role and permission management
- 👤 Employee profiles and teams
- 💼 Job posting interface
- 📄 Resume upload and analysis
- 📅 Interview scheduling interface
- 📊 Dashboard with analytics
- 📱 Mobile-responsive design

## 🛠️ Technologies Used

### Backend Stack
- **Runtime:** Node.js
- **Framework:** Express.js
- **Database:** PostgreSQL/MySQL (with Sequelize ORM)
- **Authentication:** JWT (JSON Web Tokens)
- **Security:** bcrypt, helmet
- **File Upload:** Multer
- **API Documentation:** Custom documentation
- **Environment:** dotenv

### Frontend Stack
- **Framework:** React 18
- **Language:** TypeScript
- **Build Tool:** Vite
- **Styling:** Tailwind CSS
- **UI Components:** Radix UI
- **State Management:** React Query (TanStack Query)
- **Form Handling:** React Hook Form
- **HTTP Client:** Axios
- **Routing:** React Router

## 🚀 Getting Started

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn
- PostgreSQL or MySQL database

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd "QORE Backend"
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   - Copy `.env.example` to `.env` (if available)
   - Configure your database connection
   - Set JWT secret and other environment variables

4. Create database and run migrations:
   ```bash
   npm run db:create
   npm run db:migrate
   ```

5. Seed the database (optional):
   ```bash
   npm run db:seed
   ```

6. Start the development server:
   ```bash
   npm run dev
   ```

The backend server will start on `http://localhost:3000`

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd "QORE Frontend"
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   - Configure API endpoints in `.env`
   - Set other frontend-specific variables

4. Start the development server:
   ```bash
   npm run dev
   ```

The frontend application will start on `http://localhost:5173`

## 📚 API Documentation

Comprehensive API documentation is available in the `QORE Backend/docs/` directory:

- [API Overview](QORE%20Backend/docs/api-documentation.md)
- [Authentication API](QORE%20Backend/docs/employee-auth-api.md)
- [Employees API](QORE%20Backend/docs/employees-api.md)
- [Jobs API](QORE%20Backend/docs/jobs-api.md)
- [Roles API](QORE%20Backend/docs/roles-api.md)
- [Branches API](QORE%20Backend/docs/branches-api.md)
- [And many more...](QORE%20Backend/docs/)

## 🔧 Configuration

### Backend Environment Variables
```env
# Database Configuration
DB_TYPE=postgres
DB_HOST=localhost
DB_PORT=5432
DB_NAME=qore_db
DB_USERNAME=your_username
DB_PASSWORD=your_password

# JWT Configuration
JWT_SECRET=your_jwt_secret
JWT_EXPIRES_IN=24h

# Server Configuration
PORT=3000
NODE_ENV=development

# Email Configuration
EMAIL_HOST=smtp.gmail.com
EMAIL_PORT=587
EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_app_password

# SMS Configuration
SMS_API_KEY=your_sms_api_key
```

### Frontend Environment Variables
```env
# API Configuration
VITE_API_BASE_URL=http://localhost:3000/api
VITE_APP_NAME=QORE Recruitment

# Other Configuration
VITE_UPLOAD_MAX_SIZE=10485760
```

## 🚀 Deployment

### Backend Deployment
1. Set production environment variables
2. Build the application (if using TypeScript)
3. Run database migrations in production
4. Start the server with PM2 or similar process manager

### Frontend Deployment
1. Set production environment variables
2. Build the application:
   ```bash
   npm run build
   ```
3. Deploy the `dist` folder to your hosting provider

## 📝 Available Scripts

### Backend Scripts
- `npm start` - Start production server
- `npm run dev` - Start development server with nodemon
- `npm run db:migrate` - Run database migrations
- `npm run db:seed` - Seed database with sample data
- `npm run db:reset` - Reset database (drop, create, migrate, seed)

### Frontend Scripts
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

## 🧪 Testing

### Backend Testing
```bash
cd "QORE Backend"
npm test
```

### Frontend Testing
```bash
cd "QORE Frontend"
npm test
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the ISC License - see the [LICENSE](LICENSE) file for details.

## 🙋‍♂️ Support

If you have any questions or need help with setup, please create an issue in this repository.

## 🎯 Roadmap

- [ ] Add automated testing
- [ ] Implement CI/CD pipeline
- [ ] Add Docker support
- [ ] Implement real-time notifications
- [ ] Add more integrations (LinkedIn, Indeed, etc.)
- [ ] Mobile app development

---

**Note:** This repository includes all files including `.env` configurations for development purposes. Make sure to update sensitive information before deploying to production.