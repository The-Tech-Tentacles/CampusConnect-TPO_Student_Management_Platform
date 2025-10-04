# TPO Management System

A comprehensive placement management system for engineering colleges with a **security-focused two-system architecture**.

## 🎯 **Project Overview**

This system helps colleges manage their Training and Placement Office (TPO) operations efficiently, providing **separate secure systems** for different user types.

### **Two-System Architecture:**
- **Public System**: Students & Recruiters (Internet-accessible)
- **Internal System**: TPO Admin & TPO Dept (Local network only)
- **Shared Database**: PostgreSQL with role-based permissions

## ✨ **Key Features**

### **For Students:**
- 📱 **Mobile & Web Access** - Profile management, drive applications
- 📅 **Integrated Calendar** - Placement schedules, deadlines, reminders
- 🔔 **Real-time Notifications** - Drive eligibility, application status
- 📄 **Document Management** - Resume, marksheets, certificates

### **For Recruiters:**
- 💼 **Company Portal** - Profile management, job posting
- 👥 **Candidate Management** - Application review, shortlisting
- 📊 **Analytics Dashboard** - Recruitment metrics, reports

### **For TPO Staff:**
- 🛡️ **Secure Internal System** - Local network access only
- ✅ **Verification Workflows** - Student profile, document approval
- 📅 **Calendar & Reminders** - Bulk student notifications, scheduling
- 📈 **Comprehensive Analytics** - College-wide placement insights

## 🏗️ **Technology Stack**

### **Frontend:**
- **React 18** with TypeScript
- **Material-UI** component library
- **Redux Toolkit** for state management
- **Vite** for fast development

### **Backend:**
- **FastAPI** (Python) - Two separate APIs
- **SQLAlchemy** ORM with PostgreSQL
- **JWT Authentication** with role-based access
- **Redis** for caching and sessions

### **Infrastructure:**
- **PostgreSQL 15** - Primary database
- **Redis** - Cache and session store
- **MinIO** - S3-compatible file storage
- **Docker** - Containerized development

## 🚀 **Quick Start**

### **Prerequisites:**
- Docker and Docker Compose
- Node.js 18+ (optional, for local development)
- Python 3.11+ (optional, for local development)

### **1. Clone and Setup:**
```bash
git clone <repository-url>
cd tpo-management-system
./setup.sh
```

### **2. Access the Applications:**
- **Frontend**: http://localhost:3000
- **Public API**: http://localhost:8000
- **API Documentation**: http://localhost:8000/docs
- **Database**: localhost:5432

## 📁 **Project Structure**

```
tpo-management-system/
├── 📁 frontend/              # React TypeScript application
├── 📁 backend/               # Public API (Students & Recruiters)
├── 📁 database/              # Database scripts and migrations
├── 📁 docs/                  # Technical documentation
│   ├── planning/             # Project planning documents
│   └── technical/            # Technical specifications
├── 📁 stakeholders/          # Stakeholder analysis (6 personas)
├── 📁 templates/             # Project templates
├── docker-compose.yml        # Development environment
├── PROJECT_OVERVIEW.md       # Comprehensive project summary
├── DEVELOPMENT_GUIDE.md      # Learning-focused development guide
└── README.md                 # This file
```

## 🎓 **Development Approach**

### **Learning-Focused Development:**
This project follows a **step-by-step learning approach**:
- **Concept-first**: Understand before coding
- **One block at a time**: Small, manageable pieces
- **Full explanations**: Every decision explained
- **Test and verify**: See everything working

### **Current Status:**
- ✅ **Architecture Designed** - Two-system security model
- ✅ **Documentation Complete** - Comprehensive planning
- 🔄 **Backend Development** - Learning-focused implementation
- 📋 **Next**: Database connection and authentication

## 📚 **Documentation**

### **Key Documents:**
- **PROJECT_OVERVIEW.md** - Complete project summary
- **DEVELOPMENT_GUIDE.md** - Step-by-step development approach
- **ARCHITECTURE_DECISION.md** - Security architecture reasoning
- **docs/technical/** - Complete technical specifications
- **stakeholders/** - Detailed user personas and workflows

### **Learning Resources:**
- **LEARNING_APPROACH.md** - Development methodology
- **FRESH_START_STATUS.md** - Current development status
- **Calendar Feature Specification** - Complete calendar system planning

## 🔒 **Security Features**

### **Multi-Layer Security:**
1. **Network Isolation** - Internal system not internet-accessible
2. **Database Permissions** - Different access levels per system
3. **Role-Based Access** - Granular permission control
4. **JWT Authentication** - Secure token-based auth
5. **Input Validation** - Comprehensive data sanitization

## 🛠️ **Development Commands**

### **Docker Development:**
```bash
# Start all services
docker-compose up

# View logs
docker-compose logs -f

# Restart specific service
docker-compose restart backend

# Stop all services
docker-compose down
```

### **Local Development:**
```bash
# Frontend development
cd frontend && npm install && npm run dev

# Backend development
cd backend && pip install -r requirements.txt
uvicorn main:app --reload
```

## 📊 **Project Metrics**

### **Planning Completed:**
- ✅ **6 Stakeholder Personas** - Complete user analysis
- ✅ **30+ Feature Modules** - Comprehensive feature breakdown
- ✅ **20+ Database Tables** - Production-ready schema
- ✅ **80+ API Endpoints** - Complete REST API design
- ✅ **Calendar System** - Integrated scheduling solution

### **Development Goals:**
- 🎯 **80-90% reduction** in TPO staff manual work
- 🎯 **Real-time notifications** for higher participation
- 🎯 **Automated eligibility** checking (minutes vs days)
- 🎯 **Clean verified data** for recruiter satisfaction

## 🤝 **Contributing**

This project follows a **learning-focused approach**. Contributions should:
- Include clear explanations of concepts
- Follow step-by-step implementation
- Maintain comprehensive documentation
- Prioritize security and best practices

## 📞 **Getting Help**

For questions about:
- **Architecture**: See ARCHITECTURE_DECISION.md
- **Development**: See DEVELOPMENT_GUIDE.md
- **Features**: See docs/technical/ directory
- **Security**: Review two-system architecture docs

## 📄 **License**

This project is licensed under the MIT License - see the LICENSE file for details.

---

**Ready to start learning backend development with a real-world project!** 🚀