# Pride PFP - Profile Picture Pride Flag Overlay Application

## Overview

Pride PFP is a React-based web application that allows users to add pride flag overlays to their profile pictures. The application provides a user-friendly interface for uploading images, selecting from various pride flags, customizing overlay settings, and downloading the final result. Built with modern web technologies including React, TypeScript, and Tailwind CSS, it offers a smooth and responsive user experience.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript for type safety and modern development practices
- **UI Library**: Shadcn/ui components built on Radix UI primitives for accessible, customizable components
- **Styling**: Tailwind CSS for utility-first styling with custom CSS variables for theming
- **Routing**: Wouter for lightweight client-side routing
- **State Management**: React hooks for local state, TanStack Query for server state management
- **Build Tool**: Vite for fast development and optimized production builds

### Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Language**: TypeScript with ES modules
- **Database ORM**: Drizzle ORM with PostgreSQL support (currently using in-memory storage)
- **Session Management**: Basic storage interface with expandable CRUD operations
- **Development**: TSX for TypeScript execution in development

### Canvas Processing
- **Image Processing**: HTML5 Canvas API for client-side image manipulation
- **Flag Generation**: Dynamic flag creation using gradients and color arrays
- **Overlay System**: Multiple positioning options (full, corners, center) with adjustable opacity

## Key Components

### Core Application Components
1. **ImageUpload**: Handles file upload via drag-and-drop or file selection with validation
2. **FlagSelector**: Grid-based pride flag selection with visual previews
3. **CanvasPreview**: Real-time canvas rendering with adjustment controls
4. **DownloadSection**: Export functionality with format and size options

### UI Component System
- **Shadcn/ui Components**: Complete design system with 30+ accessible components
- **Custom Styling**: CSS variables for consistent theming across light/dark modes
- **Responsive Design**: Mobile-first approach with Tailwind breakpoints

### Utility Libraries
- **Canvas Utils**: Image processing, flag generation, and overlay positioning logic
- **Flag Data**: Comprehensive pride flag database with colors and metadata
- **Query Client**: TanStack Query configuration for API communication

## Data Flow

### Image Processing Pipeline
1. **Upload**: User selects image file or chooses sample photo
2. **Validation**: File type and size validation (max 10MB, image types only)
3. **Loading**: Image loaded into HTMLImageElement for canvas processing
4. **Preview**: Real-time canvas rendering with selected flag overlay
5. **Customization**: User adjusts opacity, position, and other settings
6. **Export**: Final image generated and downloaded in chosen format

### Flag Selection Flow
1. **Display**: Grid of available pride flags with visual previews
2. **Selection**: User clicks to select desired flag
3. **Application**: Flag colors applied as gradient overlay on canvas
4. **Customization**: Position and opacity adjustments available

### State Management
- **Canvas State**: Centralized state object containing image, flag, and overlay settings
- **Component Communication**: Props-based data flow with callback functions
- **Persistence**: No server-side persistence, all processing client-side for privacy

## External Dependencies

### Frontend Libraries
- **React Ecosystem**: React 18, React DOM, React Hook Form with validation
- **UI Components**: Radix UI primitives, Lucide React icons, Class Variance Authority
- **Styling**: Tailwind CSS, clsx for conditional classes, date-fns for utilities
- **Canvas**: Embla Carousel for component carousels
- **Development**: Vite plugins for Replit integration

### Backend Libraries
- **Express**: Web framework with middleware support
- **Database**: Drizzle ORM, Neon Database serverless driver, connect-pg-simple for sessions
- **Validation**: Zod schema validation, Drizzle-Zod integration
- **Development**: tsx for TypeScript execution, esbuild for production builds

### Build and Development Tools
- **TypeScript**: Type checking and compilation
- **Vite**: Development server and build tool with React plugin
- **PostCSS**: CSS processing with Autoprefixer
- **ESBuild**: Fast JavaScript bundling for production

## Deployment Strategy

### Replit Configuration
- **Environment**: Node.js 20, Web, PostgreSQL 16 modules
- **Development**: `npm run dev` starts development server on port 5000
- **Production**: `npm run build` then `npm run start` for deployment
- **Auto-scaling**: Configured for autoscale deployment target

### Build Process
1. **Client Build**: Vite builds React application to `dist/public`
2. **Server Build**: ESBuild bundles server code to `dist/index.js`
3. **Asset Serving**: Express serves static files in production
4. **Environment**: NODE_ENV determines development vs production behavior

### Database Setup
- **Development**: In-memory storage implementation for rapid prototyping
- **Production**: PostgreSQL with Drizzle migrations via `npm run db:push`
- **Schema**: User table with username/password fields, expandable for additional features

## User Preferences

Preferred communication style: Simple, everyday language.

## Changelog

Changelog:
- June 17, 2025. Initial setup
- June 17, 2025. Complete P33ly PFP Editor implementation:
  - P33ly branding with mascot favicon and logos
  - Two custom frame options: "P33LY in Love" and "P33LY Peek"
  - Full canvas preview with real-time rendering
  - Settings panel: cutout size, shape selection, overlay opacity, frame rotation
  - Animation features with rotating frames and speed controls
  - Footer with social media links and P33ly branding
  - Enhanced slider styling with white borders for visibility
  - Download functionality with p33l_pfp.png filename
- June 17, 2025. Mobile-first responsive design implementation:
  - Comprehensive mobile optimization for primary mobile audience
  - Touch event support for hat editing on mobile devices
  - Responsive typography using clamp() for all screen sizes
  - Mobile-optimized canvas with proper aspect ratio handling
  - Improved touch targets (44px minimum) for better accessibility
  - Flexible grid layouts adapting to mobile (single column) and desktop
  - Control handles positioned precisely at hat edges for mobile interaction
  - Outside-click functionality to hide editing handles
- June 17, 2025. Final control system and GitHub preparation:
  - Three circular control buttons: Move (blue), Resize (orange), Rotate (green)
  - Buttons positioned closer to hat (25px offset) with smaller size (15px radius)
  - Mobile touch optimization with larger touch areas and smooth interactions
  - Distance-based resize control (outward = bigger, inward = smaller)
  - Removed duplicate "No Frame" option
  - Hat scaling increased to 10x maximum for bigger head profile pictures
  - Ready for professional GitHub deployment
- June 17, 2025. Dynamic control positioning system:
  - Control buttons now scale dynamically with hat size
  - 15% inset ratio from hat edges (minimum 12px for small hats)
  - Buttons stay proportionally close to hat regardless of size
  - Improved user experience for both small and large hat sizes
- June 17, 2025. GitHub preparation and documentation:
  - Created comprehensive README.md with full project documentation
  - Added detailed feature descriptions, technology stack, and usage guide
  - Included mobile optimization details and deployment instructions
  - Prepared project structure documentation for open-source release
  - Ready for GitHub upload with professional-grade documentation