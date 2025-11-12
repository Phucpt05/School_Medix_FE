# School Medix - School Health Management System

School Medix is a comprehensive school health management system built on a modern web platform, helping schools track and manage student health professionally and efficiently.

## 🌟 Key Features

### For Administrators & School Health Staff
- **User Management**: Create and manage accounts for admin, health staff, and parents
- **Health Records Management**: Track overall health information of students
- **Medical Supplies Management**: Monitor medications, consumables, and suppliers
- **Disease Management**: Record and track disease cases within the school
- **Vaccination Management**: Organize vaccination campaigns and track history
- **Regular Health Checkups**: Organize and manage health examination periods
- **Medication Management**: Process medication requests from parents
- **Statistical Reports**: Aggregate and analyze health data

### For Parents
- **Children Health Monitoring**: View health records, medical history
- **Health Declarations**: Register vaccination information, medical history
- **School Medication**: Register to send medication when children are sick
- **Schedule Tracking**: View vaccination schedules, regular health checkups
- **Notifications**: Receive updates on children's health status

## 🛠️ Technologies Used

### Frontend
- **React 19.1.0** - JavaScript library for building user interfaces
- **Vite 6.3.5** - Fast and modern frontend build tool
- **React Router DOM 7.6.2** - Navigation in React applications
- **Tailwind CSS 4.1.8** - CSS framework for responsive design
- **Lucide React 0.513.0** - Modern icon library
- **Recharts 3.1.0** - Chart library for data visualization

### Backend & Database
- **Supabase** - Backend-as-a-Service with PostgreSQL
- **Axios 1.9.0** - HTTP client for API communication

### Authentication & Security
- **Supabase Auth** - User authentication system
- **JWT Tokens** - API request authentication

### Storage & Deployment
- **Firebase Hosting** - Frontend application deployment
- **Supabase Storage** - File and image storage

### Other Libraries
- **Framer Motion 12.18.1** - Animation library
- **React Toastify 11.0.5** - User notifications
- **React PDF 10.0.1** - PDF viewing and processing
- **TipTap 2.25.0** - Rich text editor
- **Papa Parse 5.5.3** - CSV file processing

## 📁 Project Structure

```
fe/
├── public/                 # Static assets
├── src/
│   ├── components/         # Reusable components
│   │   ├── AIChat.jsx
│   │   ├── Header.jsx
│   │   ├── Footer.jsx
│   │   ├── Sidebar.jsx
│   │   └── ...
│   ├── config/            # Application configuration
│   │   ├── axiosClient.js
│   │   └── Supabase.jsx
│   ├── context/           # React Context
│   │   ├── AuthContext.jsx
│   │   └── ChildContext.js
│   ├── hooks/             # Custom React Hooks
│   ├── layouts/           # Layout components
│   │   ├── AdminLayout.jsx
│   │   ├── MainLayout.jsx
│   │   └── ParentLayout.jsx
│   ├── pages/             # Application pages
│   │   ├── Admin/         # Admin pages
│   │   ├── Parent/        # Parent pages
│   │   ├── Nurse/         # Nurse pages
│   │   ├── Auth/          # Authentication pages
│   │   └── ...
│   ├── router/            # Routing configuration
│   ├── service/           # Services
│   └── utils/             # Utility functions
├── .env                   # Environment variables
├── firebase.json         # Firebase configuration
├── package.json           # Dependencies and scripts
└── vite.config.js         # Vite configuration
```

## 🚀 Installation and Running

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn

### Steps

1. **Clone repository**
   ```bash
   git clone <repository-url>
   cd School_Medix_FE/fe
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure environment variables**
   - Create `.env` file in the `fe/` directory
   - Add the following environment variables:
   ```
   VITE_SUPABASE_URL=your_supabase_url
   VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
   ```

4. **Run application in development mode**
   ```bash
   npm run dev
   ```

5. **Build for production**
   ```bash
   npm run build
   ```

6. **Preview production build**
   ```bash
   npm run preview
   ```

## 🔧 Scripts

- `npm run dev` - Run development server
- `npm run build` - Build for production
- `npm run lint` - Run ESLint to check code
- `npm run preview` - Preview production build

## 🌐 Deployment

The application is deployed on Firebase Hosting. To deploy:

1. **Install Firebase CLI**
   ```bash
   npm install -g firebase-tools
   ```

2. **Login to Firebase**
   ```bash
   firebase login
   ```

3. **Build and deploy**
   ```bash
   npm run build
   firebase deploy
   ```

## 👥 User Roles

The system supports 3 main roles:

1. **Admin**: Manage entire system, users, and settings
2. **Nurse/Health Staff**: Manage student health, vaccinations, medical examinations
3. **Parent**: Monitor children's health, health declarations

## 📊 Dashboard

### Admin Dashboard
- Overall student health statistics
- Medical accidents and disease charts
- School health plan management
- Track medications and pending declarations

### Parent Dashboard
- List of children with notifications
- Quick access to health services
- Schedule and notification tracking

## 🔐 Security

- User authentication via Supabase Auth
- Role-based access control
- Token-based authentication for API
- Data security with HTTPS