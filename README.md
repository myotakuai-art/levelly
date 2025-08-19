# Levelly - Professional Growth Platform 🦉

Levelly is an innovative educational and gamified platform designed for entrepreneurship, side hustles, skill-building, and productivity. The platform combines AI-powered mentorship with community features and gamification to help users level up their business game.

## ✨ Features

### 🎮 Gamified Learning
- **XP System**: Earn experience points through interactions and community participation
- **Progressive Leveling**: Level up with 100 XP per level progression
- **Achievement Badges**: Unlock badges for reaching milestones and completing challenges
- **Streak Tracking**: Maintain daily learning streaks for bonus rewards
- **Leaderboards**: Compete with other entrepreneurs and track your progress

### 🤖 AI-Powered Mentorship
- **Mentor.ai**: Business strategy and entrepreneurship guidance
- **VideoAgent**: Content creation and marketing assistance
- **SalesAgent**: Sales optimization and conversion strategies
- **Persistent Chat History**: Continue conversations across sessions
- **XP Rewards**: Earn points for engaging with AI mentors

### 🌟 Community & Social Features
- **Instagram-style Feed**: Share progress, insights, and achievements
- **Image Uploads**: Post photos with your updates using object storage
- **Community Interactions**: Like, comment, and engage with other users
- **Real-time Updates**: Live community feed with WebSocket integration
- **User Profiles**: Customizable profiles with achievements and stats

### 📈 Learning & Challenges
- **Daily Challenges**: Complete entrepreneurship tasks for XP rewards
- **7-Day Programs**: Structured learning paths for specific skills
- **Progress Tracking**: Monitor your learning journey and achievements
- **Skill Development**: Build real-world business skills through gamified tasks

### 🛍️ Marketplace Integration
- **Tool Marketplace**: Discover and purchase business tools and resources
- **User-generated Content**: Sell your own resources and expertise
- **Integrated Purchasing**: Seamless transactions within the platform

## 🚀 Technology Stack

### Frontend
- **React 18** with TypeScript for type-safe development
- **Vite** for fast development and optimized builds
- **Tailwind CSS** for responsive, modern styling
- **shadcn/ui** components built on Radix UI primitives
- **TanStack Query** for efficient server state management
- **Wouter** for lightweight client-side routing

### Backend
- **Node.js** with Express.js for robust API development
- **TypeScript** throughout the entire stack
- **Drizzle ORM** for type-safe database operations
- **PostgreSQL** with Neon serverless hosting
- **WebSocket** integration for real-time features

### Authentication & Security
- **Supabase Auth** for secure user authentication
- **Multiple Auth Methods**: Email/password, Google OAuth, Replit Auth
- **Session Management**: Secure session storage with PostgreSQL
- **Protected Routes**: Comprehensive authorization system

### Infrastructure
- **Object Storage**: File uploads and asset management
- **Real-time Communication**: WebSocket server for live updates
- **Environment Management**: Secure secrets and configuration
- **Database Migrations**: Automated schema management with Drizzle

## 🛠️ Getting Started

### Prerequisites
- Node.js 18+ 
- PostgreSQL database
- Supabase project (for authentication)

### Installation

1. **Clone the repository**
```bash
git clone <your-repo-url>
cd levelly
```

2. **Install dependencies**
```bash
npm install
```

3. **Environment Setup**
Create a `.env` file with the following variables:
```env
DATABASE_URL=your_postgresql_connection_string
SUPABASE_URL=your_supabase_project_url
SUPABASE_ANON_KEY=your_supabase_anon_key
OPENAI_API_KEY=your_openai_api_key
SESSION_SECRET=your_session_secret
```

4. **Database Setup**
```bash
npm run db:push
```

5. **Start Development Server**
```bash
npm run dev
```

The application will be available at `http://localhost:5000`

## 📁 Project Structure

```
levelly/
├── client/                 # React frontend application
│   ├── src/
│   │   ├── components/    # Reusable UI components
│   │   ├── hooks/         # Custom React hooks
│   │   ├── lib/           # Utility functions and configurations
│   │   ├── pages/         # Application pages/routes
│   │   └── App.tsx        # Main application component
├── server/                # Express.js backend
│   ├── db.ts             # Database configuration
│   ├── routes.ts         # API route definitions
│   ├── storage.ts        # Database operations
│   ├── auth.ts           # Authentication middleware
│   └── index.ts          # Server entry point
├── shared/               # Shared types and schemas
│   └── schema.ts         # Database schema definitions
└── README.md             # Project documentation
```

## 🔑 Key Features Implementation

### Gamification System
- XP tracking with automatic level calculation
- Badge system stored as JSONB for flexibility
- Activity logging for progress tracking
- Leaderboard with real-time updates

### AI Integration
- OpenAI GPT-4 integration for intelligent responses
- Agent-specific system prompts for specialized guidance
- Conversation history persistence
- XP rewards for AI interactions

### Community Features
- File upload system with object storage
- Real-time feed updates via WebSocket
- User-generated content with moderation
- Social interactions (likes, comments)

### Authentication Flow
- Multi-provider authentication support
- Secure session management
- User profile synchronization
- Protected route implementation

## 🚀 Deployment

The application is optimized for deployment on Replit with:
- Automatic environment variable management
- Built-in PostgreSQL database support
- Integrated file storage solutions
- Production-ready configuration

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Commit your changes: `git commit -m 'Add amazing feature'`
4. Push to the branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🔗 Links

- [Live Demo](your-replit-url)
- [Documentation](your-docs-url)
- [Issue Tracker](your-issues-url)

---

Built with ❤️ for entrepreneurs and lifelong learners