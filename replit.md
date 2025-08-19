# Levelly - Professional Growth Platform

## Overview

Levelly is a comprehensive professional ecosystem designed for entrepreneurship, side hustles, skill-building, and productivity. The platform combines AI-powered mentorship with community features and gamification to help users level up their business game. Built as a full-stack web application, it features multiple specialized AI agents (Mentor.ai, VideoAgent, SalesAgent), real-time community interaction, user progression tracking, and WebSocket-powered live updates.

**Recent Development**: Created comprehensive blueprint for expanding into young entrepreneur marketplace and educational platform with detailed product catalog, learning modules, and AI integration strategies. Added detailed gamified learning blueprint with Duolingo-style engagement mechanics, AI mascot "Levvy", dopamine-driven features, and addictive learning paths. Successfully implemented marketplace file upload functionality with object storage integration. Created new 7-day social media & marketing growth program with higher XP rewards (10-50 XP) for practical marketing education. **Latest**: Fixed mobile navigation from 6-column to 5-column layout (Home, Community, Ranking, Profile, Quest) for better phone usability. Fixed user activities API endpoint to properly handle userId parameter and prevent 404 errors. Mobile navigation now uses fixed positioning with proper content padding.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React with TypeScript using Vite as the build tool
- **UI Framework**: shadcn/ui components built on Radix UI primitives
- **Styling**: Tailwind CSS with custom CSS variables for theming
- **State Management**: TanStack Query (React Query) for server state management
- **Routing**: Wouter for lightweight client-side routing
- **Real-time Updates**: Custom WebSocket hook for live community features

### Backend Architecture
- **Runtime**: Node.js with Express.js server
- **Language**: TypeScript with ES modules
- **Database ORM**: Drizzle ORM for type-safe database operations
- **API Architecture**: RESTful endpoints with real-time WebSocket support
- **Session Management**: Express sessions with PostgreSQL store
- **AI Integration**: OpenAI API for chat responses from specialized agents

### Database Design
- **Primary Database**: PostgreSQL with Neon serverless hosting
- **Schema Management**: Drizzle migrations and schema definitions
- **Key Tables**: Users, community posts, chat messages, user activities, sessions
- **Features**: UUID primary keys, JSONB for flexible data (badges, metadata), timestamp tracking

### Authentication & Authorization
- **Provider**: Replit Auth with OpenID Connect
- **Session Storage**: PostgreSQL-backed sessions with connect-pg-simple
- **Security**: HTTP-only cookies, CSRF protection, secure session configuration
- **User Management**: Automatic user creation/updates on authentication

### Real-time Features
- **WebSocket Server**: Custom WebSocket implementation for live updates
- **Use Cases**: Community feed updates, chat responses, XP/badge notifications
- **Architecture**: Room-based messaging for targeted user updates

### AI Agent System
- **Three Specialized Agents**: 
  - Mentor.ai (business mentorship)
  - VideoAgent (content creation)
  - SalesAgent (sales optimization)
- **Chat Architecture**: Persistent conversation history with XP rewards
- **Response Generation**: OpenAI GPT-4o with agent-specific system prompts

### Gamification System
- **XP System**: Points earned through interactions, community participation
- **Leveling**: Progressive level system with 100 XP per level
- **Badges**: Achievement system stored as JSONB array
- **Leaderboard**: User ranking based on total XP earned

## External Dependencies

### Core Services
- **Neon Database**: Serverless PostgreSQL hosting for primary data storage
- **OpenAI API**: GPT-4o model for AI agent conversations and responses
- **Replit Auth**: Authentication provider using OpenID Connect protocol

### UI/UX Libraries
- **Radix UI**: Headless component primitives for accessibility
- **Tailwind CSS**: Utility-first CSS framework for styling
- **Lucide React**: Icon library for consistent iconography
- **date-fns**: Date formatting and manipulation utilities

### Development Tools
- **Vite**: Frontend build tool and development server
- **TypeScript**: Type safety across frontend and backend
- **ESBuild**: Fast JavaScript bundler for production builds
- **Drizzle Kit**: Database migrations and schema management CLI

### Runtime Dependencies
- **TanStack Query**: Async state management and caching
- **WebSocket (ws)**: Real-time bidirectional communication
- **React Hook Form**: Form state management with validation
- **Zod**: Runtime type validation and schema parsing