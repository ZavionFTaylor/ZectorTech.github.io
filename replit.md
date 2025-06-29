# Zector Technology LLC - Robotics Solutions Platform

## Overview

This is a full-stack web application for Zector Technology LLC, a professional robotics solutions company. The application is built as a modern single-page application (SPA) that showcases the company's services, portfolio, and provides a contact system for potential clients. The architecture follows a typical React frontend with Express.js backend pattern, utilizing modern development tools and frameworks.

## System Architecture

The application follows a monorepo structure with clear separation between client and server components:

- **Frontend**: React-based SPA with TypeScript, using Vite as the build tool
- **Backend**: Express.js server with TypeScript support
- **Database**: PostgreSQL with Drizzle ORM for type-safe database operations
- **UI Framework**: Tailwind CSS with shadcn/ui component library for consistent design
- **State Management**: TanStack Query for server state management
- **Routing**: Wouter for client-side routing

## Key Components

### Frontend Architecture
- **React 18** with TypeScript for type safety
- **Vite** for fast development and optimized builds
- **Tailwind CSS** for utility-first styling with custom design tokens
- **shadcn/ui** component library for consistent UI components
- **TanStack Query** for efficient server state management and caching
- **Wouter** for lightweight client-side routing
- **React Hook Form** for form management and validation

### Backend Architecture
- **Express.js** server with TypeScript
- **Drizzle ORM** for database operations with PostgreSQL
- **Zod** for runtime type validation and schema generation
- **Session management** with connect-pg-simple for PostgreSQL session store
- **RESTful API** structure with middleware for logging and error handling

### Database Schema
- **Users table**: Basic user management with username/password authentication
- **PostgreSQL**: Chosen for reliability and advanced features
- **Drizzle migrations**: Version-controlled database schema changes

### UI/UX Design
- **Professional branding**: Red and gold color scheme matching company identity
- **Responsive design**: Mobile-first approach with adaptive layouts
- **Component-based architecture**: Reusable UI components for maintainability
- **Accessibility**: Built with screen readers and keyboard navigation in mind

## Data Flow

1. **Client Requests**: React components make API calls through TanStack Query
2. **Server Processing**: Express.js routes handle business logic and database operations
3. **Database Operations**: Drizzle ORM provides type-safe database interactions
4. **Response Handling**: JSON responses with proper error handling and logging
5. **State Management**: TanStack Query manages caching and synchronization

## External Dependencies

### Core Framework Dependencies
- **@neondatabase/serverless**: Neon PostgreSQL serverless driver
- **drizzle-orm**: Type-safe ORM for database operations
- **@tanstack/react-query**: Server state management
- **@radix-ui/***: Headless UI components for accessibility

### Development Tools
- **Vite**: Fast build tool with HMR support
- **TypeScript**: Static type checking across the entire stack
- **ESLint/Prettier**: Code quality and formatting (implied by structure)
- **PostCSS**: CSS processing with Tailwind integration

### External Services
- **Neon Database**: Serverless PostgreSQL hosting
- **Replit**: Development and hosting platform integration
- **Font Awesome & Google Fonts**: Icon and typography resources

## Deployment Strategy

### Development Environment
- **Vite dev server**: Hot module replacement for rapid development
- **Express server**: Concurrent development with API proxy
- **Database migrations**: Automated schema updates with Drizzle

### Production Build
- **Client build**: Vite optimizes and bundles React application
- **Server build**: ESBuild compiles TypeScript server code
- **Static assets**: Served from Express with proper caching headers
- **Environment variables**: DATABASE_URL and other config managed via environment

### Replit Integration
- **Development banner**: Automatic injection for development mode
- **Runtime error overlay**: Enhanced debugging in development
- **Cartographer plugin**: Development tooling integration

## Changelog

- June 29, 2025. Initial setup

## User Preferences

Preferred communication style: Simple, everyday language.