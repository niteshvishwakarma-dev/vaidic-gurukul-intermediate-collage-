# Vaidic Gurukul - College Website & Management System

A comprehensive, professional-grade college website and student management system built with modern web technologies.

## Project Overview

This is a complete educational institution digital platform featuring:
- Public-facing college website
- Secure admin dashboard
- Student portal
- Faculty management system
- Complete college management module
- Role-based access control
- Advanced reporting and analytics

## Technology Stack

### Frontend
- **Framework**: Next.js 14+ (React)
- **Styling**: Tailwind CSS
- **UI Components**: Custom + Shadcn/ui
- **Icons**: Lucide React
- **Forms**: React Hook Form + Zod validation
- **State Management**: React Context + Zustand
- **Charts**: Recharts
- **HTTP Client**: Axios

### Backend
- **Runtime**: Node.js
- **Framework**: Express.js
- **Authentication**: JWT + bcrypt
- **Middleware**: Custom auth, role-based access
- **Validation**: Joi/Zod
- **File Upload**: Multer

### Database
- **Primary DB**: PostgreSQL
- **ORM**: Sequelize/TypeORM
- **Migrations**: TypeORM/Sequelize migrations

### DevOps & Tools
- **Version Control**: Git
- **Package Manager**: npm/yarn
- **Environment**: .env configuration
- **API Testing**: Postman/Thunder Client

## Project Structure

```
vaidic-gurukul/
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── app/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── layouts/
│   │   ├── hooks/
│   │   ├── services/
│   │   ├── utils/
│   │   ├── types/
│   │   ├── store/
│   │   └── styles/
│   ├── package.json
│   └── next.config.js
│
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── routes/
│   │   ├── middleware/
│   │   ├── models/
│   │   ├── services/
│   │   ├── validators/
│   │   ├── utils/
│   │   ├── config/
│   │   └── app.js
│   ├── database/
│   │   ├── migrations/
│   │   └── seeders/
│   ├── package.json
│   └── .env.example
│
├── docs/
│   ├── API.md
│   ├── DATABASE.md
│   ├── SETUP.md
│   └── DEPLOYMENT.md
│
└── .gitignore
```

## Features

### Public Website
- ✅ Home page with hero section
- ✅ About college
- ✅ Academics & courses
- ✅ Departments
- ✅ Admissions
- ✅ Events & news
- ✅ Gallery
- ✅ Contact & feedback
- ✅ SEO optimized
- ✅ Responsive design

### Admin Dashboard
- ✅ Analytics & statistics
- ✅ Student management
- ✅ Faculty management
- ✅ Course & department management
- ✅ Attendance tracking
- ✅ Examination management
- ✅ Fee management
- ✅ Notice board
- ✅ Event management
- ✅ Document management
- ✅ CMS for website content
- ✅ Reports & exports

### Student Portal
- ✅ Dashboard with overview
- ✅ Profile management
- ✅ Course enrollment
- ✅ Attendance tracking
- ✅ Assignment submission
- ✅ Exam schedules & results
- ✅ Fee status tracking
- ✅ Notice board
- ✅ Notifications
- ✅ Support tickets

### Faculty Portal
- ✅ Class management
- ✅ Attendance marking
- ✅ Assignment management
- ✅ Mark entry
- ✅ Notice posting
- ✅ Student communication

### Security
- ✅ JWT authentication
- ✅ Role-based access control
- ✅ Password hashing (bcrypt)
- ✅ Input validation
- ✅ SQL injection protection
- ✅ XSS protection
- ✅ CSRF protection
- ✅ Rate limiting

## Getting Started

### Prerequisites
- Node.js 16+
- PostgreSQL 12+
- npm or yarn

### Installation

1. **Clone repository**
```bash
git clone https://github.com/niteshvishwakarma-dev/vaidic-gurukul-intermediate-collage-.git
cd vaidic-gurukul-intermediate-collage-
```

2. **Setup Backend**
```bash
cd backend
npm install
cp .env.example .env
# Edit .env with your database credentials
npm run migrate
npm run seed
npm start
```

3. **Setup Frontend**
```bash
cd ../frontend
npm install
cp .env.local.example .env.local
# Edit .env.local with API URL
npm run dev
```

4. **Access Application**
- Public Website: http://localhost:3000
- Admin Panel: http://localhost:3000/admin
- API: http://localhost:5000/api

## Default Credentials (Development Only)

### Admin
- Email: admin@vaidic.com
- Password: Admin@123

### Faculty
- Email: faculty@vaidic.com
- Password: Faculty@123

### Student
- Email: student@vaidic.com
- Password: Student@123

## Database Schema

See `docs/DATABASE.md` for complete database schema and relationships.

Key tables:
- users (with roles: admin, faculty, student)
- students
- faculty
- departments
- courses
- subjects
- enrollment
- attendance
- assignments
- exam_results
- fees
- payments
- notices
- events
- admissions

## API Documentation

See `docs/API.md` for complete API endpoint documentation.

Base URL: `http://localhost:5000/api`

Examples:
- `POST /auth/login` - User login
- `GET /students` - List students (admin only)
- `GET /courses` - List courses
- `POST /admissions/apply` - Submit admission application

## Development

### Frontend Development
```bash
cd frontend
npm run dev        # Start dev server
npm run build      # Build for production
npm run lint       # Run linter
```

### Backend Development
```bash
cd backend
npm run dev        # Start with nodemon
npm run build      # Build for production
npm test           # Run tests
```

## Deployment

See `docs/DEPLOYMENT.md` for detailed deployment instructions for:
- Vercel (Frontend)
- Railway/Heroku (Backend)
- Database setup on production server

## Security Notes

- Never commit `.env` files
- Always use HTTPS in production
- Enable CORS only for trusted domains
- Implement rate limiting
- Use environment variables for sensitive data
- Regularly update dependencies
- Implement proper logging and monitoring

## Contributing

Contribution guidelines to be added.

## License

Private project for Vaidic Gurukul College.

## Support

For issues and questions, contact: support@vaidic.com

---

**Build with ❤️ for education**
