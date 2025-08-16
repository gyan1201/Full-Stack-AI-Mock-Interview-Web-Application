<<<<<<< HEAD
# Full-Stack AI Mock Interview Platform  

A modern, Full-Stack AI Mock Interview Platform application built with Next.js 13, TypeScript, Tailwind CSS, and Prisma. This application demonstrates best practices for building scalable web applications with modern technologies.

## Features

- **User Authentication**: Secure user registration and login with NextAuth.js
- **Blog Posts**: Create, read, and manage blog posts
- **Categories**: Organize posts with categories
- **Comments**: Interactive commenting system on posts
- **Responsive Design**: Modern UI built with Tailwind CSS
- **Type Safety**: Full TypeScript support throughout the application
- **Database**: PostgreSQL database with Prisma ORM
- **API Routes**: RESTful API endpoints for all functionality

## Tech Stack

- **Frontend**: Next.js 13 (App Router), React 18, TypeScript
- **Styling**: Tailwind CSS
- **Authentication**: NextAuth.js
- **Database**: PostgreSQL with Prisma ORM
- **Forms**: React Hook Form with Zod validation
- **Icons**: Heroicons (SVG)

## Prerequisites

Before running this application, make sure you have:

- Node.js 18+ installed
- PostgreSQL database running
- npm or yarn package manager

## Getting Started

### 1. Clone and Install Dependencies

```bash
cd fullstack-app
npm install
```

### 2. Environment Setup

Create a `.env` file in the root directory with the following variables:

```env
DATABASE_URL="postgresql://username:password@localhost:5432/fullstack_app"
NEXTAUTH_SECRET="your-secret-key-here"
NEXTAUTH_URL="http://localhost:3000"
```

**Important**: Replace the placeholder values with your actual database credentials and generate a secure secret key.

### 3. Database Setup

```bash
# Generate Prisma client
npx prisma generate

# Run database migrations
npx prisma migrate dev --name init

# (Optional) Seed the database with sample data
npx prisma db seed
```

### 4. Run the Application

```bash
# Development mode
npm run dev

# Build for production
npm run build
npm start
```

The application will be available at `http://localhost:3000`

## Project Structure

```
src/
├── app/                    # Next.js 13 app directory
│   ├── api/               # API routes
│   │   ├── auth/          # Authentication endpoints
│   │   ├── posts/         # Post management endpoints
│   │   └── categories/    # Category management endpoints
│   ├── auth/              # Authentication pages
│   ├── posts/             # Post-related pages
│   └── create-post/       # Post creation page
├── components/             # Reusable React components
├── lib/                    # Utility functions and configurations
└── types/                  # TypeScript type definitions
```

## API Endpoints

### Authentication
- `POST /api/register` - User registration
- `GET/POST /api/auth/[...nextauth]` - NextAuth.js endpoints

### Posts
- `GET /api/posts` - Fetch all published posts
- `POST /api/posts` - Create a new post
- `GET /api/posts/[id]/comments` - Fetch comments for a post
- `POST /api/posts/[id]/comments` - Add a comment to a post

### Categories
- `GET /api/categories` - Fetch all categories
- `POST /api/categories` - Create a new category (admin only)

## Database Schema

The application uses the following main models:

- **User**: User accounts with authentication
- **Post**: Blog posts with content and metadata
- **Category**: Post categories for organization
- **Comment**: User comments on posts

## Features in Detail

### User Authentication
- Secure password hashing with bcrypt
- JWT-based sessions with NextAuth.js
- Protected routes and API endpoints
- User role management (User/Admin)

### Blog Management
- Rich text post creation
- Category organization
- Draft/publish functionality
- Author attribution

### Comment System
- Real-time comment posting
- User authentication required
- Comment threading support
- Moderation capabilities

### Responsive Design
- Mobile-first approach
- Modern UI components
- Smooth transitions and animations
- Accessible design patterns

## Development

### Code Quality
- ESLint configuration for code quality
- TypeScript strict mode enabled
- Consistent code formatting
- Component-based architecture

### Database Development
```bash
# Open Prisma Studio for database management
npx prisma studio

# Reset database (development only)
npx prisma migrate reset

# Generate new migration
npx prisma migrate dev --name migration_name
```

### Testing
```bash
# Run tests (when implemented)
npm test

# Run tests in watch mode
npm run test:watch
```

## Deployment

### Environment Variables
Ensure all environment variables are properly set in your production environment:

- `DATABASE_URL`: Production PostgreSQL connection string
- `NEXTAUTH_SECRET`: Secure random string for JWT signing
- `NEXTAUTH_URL`: Your production domain

### Database
- Use a managed PostgreSQL service (e.g., Supabase, PlanetScale, AWS RDS)
- Set up proper database backups
- Configure connection pooling for production

### Build and Deploy
```bash
# Build the application
npm run build

# Start production server
npm start
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## License

This project is open source and available under the [MIT License](LICENSE).

## Support

If you encounter any issues or have questions:

1. Check the [Issues](https://github.com/yourusername/fullstack-app/issues) page
2. Create a new issue with detailed information
3. Review the documentation and code examples

## Acknowledgments

- Next.js team for the amazing framework
- Prisma team for the excellent ORM
- Tailwind CSS team for the utility-first CSS framework
- NextAuth.js team for authentication solutions

---

Built with ❤️ using modern web technologies
=======
#  Full-Stack AI Mock Interview Platform  

An end-to-end **AI-powered SaaS application** built from scratch to help users **prepare for job interviews** with realistic **AI-driven mock interview sessions**.  

The platform features a **live streaming AI avatar interviewer**, **real-time feedback**, and a **subscription model**, combining the power of AI with modern full-stack development practices.  

---

##  Key Features  

###  AI-Driven Interview Generation  
- Generates interview questions based on **uploaded resumes (PDF)** or **job descriptions**.  
- Automated workflows powered by **n8n** for drag-and-drop orchestration.  
- **ImageKit** integration for free cloud storage and resume text extraction.  
- **OpenAI / Gemini** models generate tailored interview questions + analyze conversations.  

###  Interactive Interview Experience  
- **Akool Streaming Avatar API** conducts **live interviews** with real-time interaction.  
- Displays **conversation transcripts** during sessions.  
- In-call controls: **mute/unmute** and **end call**.  

###  Automated Feedback & Reporting  
- Generates **detailed feedback** (strengths, suggestions, rating out of 10).  
- Uses **n8n AI workflows** to process interview conversations.  
- Feedback stored in user dashboard for review anytime.  

###  User Management & Security  
- **Clerk** for secure authentication (Gmail, email/password, social login).  
- Subscription billing with free & paid tiers (limit free users to 2 interviews/day).  
- **Arja** for rate limiting, bot detection, email validation, and attack prevention.  

###  Scalable Data Infrastructure  
- **Convex DB** (real-time, open-source) for storing sessions, users, and app data.  
- Designed schemas for **user profiles & interview sessions** with relationships.  

###  Modern Web Development Stack  
- **React + Next.js** (folder-based routing, RSC, client/server rendering).  
- **Tailwind CSS** + **ShadCN** + **Aceternity UI** for sleek UI.  
- **React Context API** for global state management.  
- **TypeScript** for type safety and code quality.  

###  Deployment & Production Readiness  
- Deployed frontend to **Vercel** with CI/CD.  
- **n8n workflows** deployed on **Hostinger** for scalable AI automation.  

---

##  Tech Stack  

- **Frontend**: React, Next.js, Tailwind CSS, ShadCN, Aceternity UI  
- **Backend/Automation**: n8n, OpenAI/Gemini, Convex DB  
- **Auth & Billing**: Clerk (OAuth, MFA, Stripe billing)  
- **AI Avatar**: Akool API (live streaming interviews)  
- **Storage**: ImageKit (resume storage & parsing)  
- **Security**: Arja (rate limiting, bot detection)  
- **Deployment**: Vercel (frontend), Hostinger (n8n workflows)  

---

##  Screenshots  


>>>>>>> 8feaa6c678fa4575ee4f2ea099b42b8bbc2f1c2b
