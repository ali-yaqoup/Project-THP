# Backend Setup Guide for THP Platform

## 🚨 Important: Backend Required

The THP (Talent Hiring Platform) frontend application requires a backend API to function properly. The frontend is configured to connect to a backend running on `http://localhost:8000/api`.

## 🔗 Backend Repository

The official backend repository is available at:
**https://github.com/ali-yaqoup/backend-THP1.git**

## 📋 Backend Requirements

### API Endpoints Configuration

The frontend expects the following API endpoints:

#### Authentication Endpoints
- `POST /api/register` - User registration
- `POST /api/login-step1` - First step of login
- `POST /api/login-step2` - Second step of login
- `POST /api/password/send-otp` - Send password reset OTP
- `POST /api/password/reset` - Reset password
- `GET /api/user` - Get user information
- `GET /api/email/verify/{id}/{hash}` - Email verification

#### Job Management Endpoints
- Job posting CRUD operations
- Job bidding system
- User management
- Admin dashboard data

### Database Requirements
- User authentication system
- Job postings storage
- Bidding system
- User roles and permissions

## 🛠️ Backend Setup Instructions

### 1. Clone Backend Repository
```bash
git clone https://github.com/ali-yaqoup/backend-THP1.git
cd backend-THP1
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Configure Environment
- Set up database connection
- Configure API endpoints
- Set up environment variables

### 4. Run Backend Server
```bash
npm start
# Backend should run on http://localhost:8000
```

## 🔧 Frontend Configuration

### API Base URL
The frontend is configured to connect to:
```typescript
private apiUrl = 'http://localhost:8000/api';
```

### Token Management
- JWT tokens stored in localStorage
- Automatic token injection via HTTP interceptors
- Authentication state management

## 🚀 Full Stack Deployment

### Development Environment
1. **Backend**: Run on port 8000
2. **Frontend**: Run on port 4200
3. **Database**: Configure as needed

### Production Environment
1. **Backend**: Deploy to your preferred hosting
2. **Frontend**: Build and deploy to static hosting
3. **API URL**: Update frontend API configuration

## 📝 Notes for Upwork Clients

### What's Included
- ✅ Complete frontend application
- ✅ All UI components and pages
- ✅ Authentication flow (frontend)
- ✅ Job management interface
- ✅ Admin dashboard UI
- ✅ Data visualization components

### What's Not Included
- ❌ Backend API implementation
- ❌ Database setup
- ❌ Server deployment
- ❌ Production hosting

### Backend Integration
The frontend is fully prepared for backend integration with:
- HTTP client services
- Authentication interceptors
- Token management
- Error handling
- API response handling

### Next Steps
1. Set up the backend repository
2. Configure database
3. Deploy backend to your preferred hosting
4. Update frontend API URL if needed
5. Test full integration

---

**For complete functionality, both frontend and backend must be running simultaneously.**
