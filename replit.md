# AgriAssist - Smart Farming Solutions

## Overview

AgriAssist is a comprehensive agricultural technology platform designed to empower farmers with AI-powered tools for crop disease diagnosis, market analysis, and government scheme navigation. The application provides a modern, accessible interface for farmers to make informed decisions about their agricultural practices.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript
- **Styling**: Tailwind CSS with custom design system
- **UI Components**: Radix UI primitives with shadcn/ui components
- **State Management**: TanStack Query for server state management
- **Routing**: Wouter for client-side routing
- **Build Tool**: Vite with TypeScript support

### Backend Architecture
- **Runtime**: Node.js with Express.js
- **Language**: TypeScript with ESM modules
- **Database**: PostgreSQL with Drizzle ORM
- **Database Provider**: Neon Database (serverless PostgreSQL)
- **File Upload**: Multer for image processing
- **AI Integration**: Google Gemini AI for crop analysis

### Design System
- **Component Library**: Custom components built on Radix UI
- **Theme**: New York style with neutral color palette
- **Typography**: PT Sans font family
- **Responsive Design**: Mobile-first approach with Tailwind breakpoints

## Key Components

### 1. Crop Disease Diagnosis
- **Purpose**: AI-powered crop disease detection and treatment recommendations
- **Technology**: Google Gemini AI for image analysis
- **Features**: 
  - Image upload and preprocessing
  - Disease identification with confidence scores
  - Treatment and prevention recommendations
  - Diagnosis history storage

### 2. Market Analysis
- **Purpose**: Real-time crop pricing and market insights
- **Features**:
  - Live market price tracking
  - Price trend analysis
  - Market insights generation
  - Multi-crop price comparison

### 3. Government Schemes
- **Purpose**: Navigation and information about agricultural schemes
- **Features**:
  - Scheme categorization (Direct Benefit Transfer, Equipment Subsidy, Insurance, Training)
  - Eligibility criteria display
  - Application process guidance
  - Benefits overview

### 4. Voice Interface
- **Purpose**: Accessibility for farmers with limited literacy
- **Technology**: Web Speech API for recognition and synthesis
- **Features**:
  - Voice command recognition
  - Text-to-speech feedback
  - Multi-language support planning

## Data Flow

### Image Analysis Flow
1. User uploads crop image via web interface
2. Multer middleware processes and stores image
3. Image sent to Google Gemini AI for analysis
4. AI returns structured diagnosis with confidence scores
5. Results stored in PostgreSQL database
6. Formatted response sent to frontend

### Market Data Flow
1. Static market data serves as baseline
2. Periodic updates simulate real-time price changes
3. TanStack Query manages client-side caching
4. Market insights generated via AI analysis

### Government Schemes Flow
1. Static scheme data stored in database
2. Categorized display with filtering capabilities
3. Search and filter functionality for scheme discovery

## External Dependencies

### AI Services
- **Google Gemini AI**: Primary AI service for crop analysis and market insights
- **Configuration**: API key-based authentication
- **Fallback**: Error handling for API failures

### Database
- **Neon Database**: Serverless PostgreSQL provider
- **Connection**: Environment variable-based configuration
- **Migrations**: Drizzle Kit for schema management

### Third-Party Libraries
- **UI Components**: Extensive Radix UI ecosystem
- **Form Handling**: React Hook Form with Zod validation
- **Date Handling**: date-fns for date operations
- **Styling**: Tailwind CSS with custom configuration

## Deployment Strategy

### Build Process
1. **Frontend**: Vite builds React application to static assets
2. **Backend**: esbuild bundles Node.js server code
3. **Database**: Drizzle migrations ensure schema consistency

### Environment Configuration
- **Development**: Local development with hot reload
- **Production**: Optimized builds with environment-specific settings
- **Database**: Environment-based connection strings

### File Structure
```
├── client/          # React frontend application
├── server/          # Express backend application
├── shared/          # Shared TypeScript types and schemas
├── migrations/      # Database migration files
└── uploads/         # File upload storage
```

## Changelog

```
Changelog:
- July 04, 2025. Initial setup
```

## User Preferences

```
Preferred communication style: Simple, everyday language.
```