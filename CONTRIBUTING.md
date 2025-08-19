# Contributing to Levelly

Thank you for your interest in contributing to Levelly! This document provides guidelines and information for contributors.

## 🚀 Getting Started

### Prerequisites
- Node.js 18 or higher
- Git
- PostgreSQL (or use Neon serverless)
- Supabase account for authentication

### Development Setup
1. Fork the repository
2. Clone your fork: `git clone https://github.com/yourusername/levelly.git`
3. Install dependencies: `npm install`
4. Set up environment variables (see README.md)
5. Run the development server: `npm run dev`

## 📝 How to Contribute

### Reporting Bugs
- Use the GitHub issue tracker
- Include clear description and steps to reproduce
- Provide environment details (OS, Node.js version, etc.)
- Add screenshots if applicable

### Suggesting Features
- Open an issue with the "enhancement" label
- Describe the feature and its use case
- Explain how it fits with the current system

### Code Contributions

#### Branch Naming
- `feature/description` - New features
- `fix/description` - Bug fixes  
- `docs/description` - Documentation updates
- `refactor/description` - Code refactoring

#### Commit Messages
Follow conventional commits:
- `feat: add new gamification feature`
- `fix: resolve authentication bug`
- `docs: update API documentation`
- `style: format code with prettier`

#### Pull Request Process
1. Create a new branch from `main`
2. Make your changes
3. Test thoroughly
4. Update documentation if needed
5. Submit a pull request

### Code Style

#### TypeScript
- Use TypeScript for all new code
- Maintain strong typing throughout
- Use proper interfaces and types

#### React Components
- Use functional components with hooks
- Follow component naming conventions (PascalCase)
- Keep components focused and reusable

#### Backend
- Use async/await instead of callbacks
- Implement proper error handling
- Add logging for debugging

#### Database
- Use Drizzle ORM for all database operations
- Write migrations for schema changes
- Follow naming conventions (snake_case for columns)

## 🧪 Testing

### Running Tests
```bash
npm test
```

### Writing Tests
- Write unit tests for utilities and business logic
- Test React components with React Testing Library
- Include integration tests for API endpoints

## 📚 Documentation

### Code Documentation
- Add JSDoc comments for complex functions
- Include usage examples
- Document API endpoints

### User Documentation
- Update README.md for new features
- Include screenshots for UI changes
- Write clear installation instructions

## 🔍 Code Review Process

### For Contributors
- Ensure your code follows the style guidelines
- Include tests for new functionality
- Update documentation as needed
- Keep pull requests focused and small

### For Reviewers
- Check functionality and code quality
- Verify tests pass and coverage is adequate
- Ensure documentation is updated
- Test the changes locally

## 🎯 Development Priorities

### High Priority
- User authentication and security
- Core gamification features
- AI integration stability
- Mobile responsiveness

### Medium Priority
- Advanced community features
- Marketplace functionality
- Analytics and reporting
- Performance optimizations

### Low Priority
- UI polish and animations
- Advanced customization options
- Additional integrations

## 🛠️ Architecture Guidelines

### Frontend
- Use React Query for server state
- Implement proper loading and error states
- Follow mobile-first responsive design
- Use shadcn/ui components when possible

### Backend
- Implement proper authentication middleware
- Use database transactions for data consistency
- Add rate limiting for API endpoints
- Implement comprehensive logging

### Database
- Design efficient schema relationships
- Use indexes for performance
- Implement proper data validation
- Follow data privacy best practices

## 📞 Getting Help

### Communication Channels
- GitHub Issues for bugs and features
- Discussions for questions and ideas
- Code reviews for implementation feedback

### Response Times
- Issues: Within 48 hours
- Pull requests: Within 72 hours
- Security issues: Within 24 hours

## 🏆 Recognition

Contributors will be recognized in:
- README.md contributors section
- Release notes for significant contributions
- Special badges for long-term contributors

Thank you for helping make Levelly better for everyone!