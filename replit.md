# LinguaFlow Translation Platform

## Overview

LinguaFlow is a comprehensive AI-powered translation platform that provides text translation, document processing, audio transcription, and language learning capabilities. The application is built as a full-stack TypeScript solution with a React frontend and Express.js backend, designed for professional translators, teams, and language learners.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript using Vite as the build tool
- **UI Components**: Radix UI primitives with shadcn/ui design system
- **Styling**: Tailwind CSS with custom CSS variables for theming
- **State Management**: TanStack Query (React Query) for server state and caching
- **Routing**: Wouter for lightweight client-side routing
- **Form Handling**: React Hook Form with Zod validation

### Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Language**: TypeScript with ES modules
- **API Design**: RESTful endpoints with standardized error handling
- **Database**: PostgreSQL with Drizzle ORM for type-safe database operations
- **AI Integration**: OpenAI GPT-4 for translation and language processing tasks

### Database Architecture
- **Schema Design**: Comprehensive relational schema supporting users, translations, documents, audio transcriptions, glossaries, translation memory, teams, and projects
- **ORM**: Drizzle ORM with automatic TypeScript type generation
- **Migrations**: Database versioning through drizzle-kit
- **Connection**: Neon serverless PostgreSQL for scalable cloud database

### Authentication & Authorization
- **Mock Authentication**: Development uses mock user ID for simplified testing
- **Session Management**: Designed for session-based authentication (implementation pending)
- **User Management**: User profiles with plan-based access control

### Core Features Architecture

#### Translation Engine
- **Multi-model Support**: OpenAI GPT-4 and DeepL integration
- **Context Enhancement**: Glossary terms and translation memory integration
- **Quality Feedback**: User rating system for translation improvement
- **Language Support**: 15+ language pairs with cultural localization

#### Document Processing
- **File Upload**: Support for document translation workflows
- **Content Extraction**: Text processing from various document formats
- **Batch Processing**: Designed for large document translation jobs

#### Audio Processing
- **Speech Recognition**: Web Speech API integration for real-time transcription
- **Audio File Processing**: Upload and transcribe audio files
- **Language Detection**: Automatic language identification for audio content

#### Collaboration Features
- **Team Management**: Multi-user team collaboration with role-based access
- **Project Organization**: Project-based workflow management
- **Translation Memory**: Shared translation memory across teams
- **Glossary Management**: Collaborative terminology management

### External Dependencies

#### AI Services
- **OpenAI API**: GPT-4 for advanced translation and language processing
- **DeepL API**: Professional translation service integration
- **Web Speech API**: Browser-native speech recognition

#### Database Services
- **Neon Database**: Serverless PostgreSQL hosting
- **Drizzle ORM**: Type-safe database operations and migrations

#### UI/UX Libraries
- **Radix UI**: Accessible component primitives
- **Tailwind CSS**: Utility-first CSS framework
- **Lucide React**: Consistent icon library
- **TanStack Query**: Server state management and caching

#### Development Tools
- **Vite**: Fast development server and build tool
- **TypeScript**: Type safety and developer experience
- **ESLint/Prettier**: Code quality and formatting
- **Replit Integration**: Cloud development environment support

#### Deployment Infrastructure
- **Build System**: Vite for frontend, esbuild for backend
- **Environment**: Node.js runtime with ES module support
- **Static Assets**: Vite-optimized asset bundling and serving