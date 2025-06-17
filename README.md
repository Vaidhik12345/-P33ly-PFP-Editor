# P33ly PFP Editor

A dynamic web application for creating personalized profile picture overlays with P33ly-themed hats and frames. Built with React, TypeScript, and Canvas API for professional-grade image editing.

![P33ly PFP Editor](https://via.placeholder.com/800x400/1a1a1a/ff4a00?text=P33ly+PFP+Editor)

## ✨ Features

### Core Functionality
- **Image Upload**: Drag-and-drop or click to upload profile pictures (up to 10MB)
- **Hat Selection**: 4 unique P33ly-themed hats including MNFA Cap, Cool Hat (sunglasses), and In Love Hat (heart eyes)
- **Frame Options**: Choose from "No Frame", "P33LY in Love", and "P33LY Peek" decorative frames
- **Real-time Preview**: Live canvas rendering with instant feedback

### Advanced Controls
- **Ultra-smooth Hat Editing**: Professional-grade controls with 120fps responsiveness
- **Triangle Control Layout**: Move (top-left), Resize (top-right), Rotate (bottom-center)
- **Momentum-based Movement**: Smooth animations with easing curves
- **Dynamic Positioning**: Control buttons scale with hat size for optimal UX

### Customization Options
- **Hat Scaling**: Resize from 20% to 1000% with precision control
- **Rotation**: Full 360° rotation with degree precision
- **Position Adjustment**: Fine-tune horizontal and vertical placement
- **Frame Settings**: Cutout size, shape selection (circle/square), overlay opacity
- **Animation**: Rotating frames with adjustable speed controls

### Mobile-First Design
- **Touch Optimized**: Enhanced touch interactions for mobile devices
- **Responsive Layout**: Adapts seamlessly from mobile to desktop
- **44px Touch Targets**: Accessibility-compliant interactive elements
- **Momentum Scrolling**: Smooth mobile navigation experience

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ and npm
- Modern web browser with Canvas API support

### Installation
```bash
# Clone the repository
git clone https://github.com/yourusername/p33ly-pfp-editor.git
cd p33ly-pfp-editor

# Install dependencies
npm install

# Start development server
npm run dev
```

### Production Build
```bash
# Build for production
npm run build

# Start production server
npm run start
```

## 🛠️ Technology Stack

### Frontend
- **React 18** with TypeScript for type-safe development
- **Tailwind CSS** for utility-first styling with custom P33ly theme
- **Wouter** for lightweight client-side routing
- **TanStack Query** for server state management
- **Shadcn/ui** components built on Radix UI primitives

### Backend
- **Express.js** with TypeScript
- **Drizzle ORM** with PostgreSQL support
- **In-memory storage** for development (expandable to full database)

### Build & Development
- **Vite** for fast development and optimized builds
- **ESBuild** for production bundling
- **PostCSS** with Autoprefixer for CSS processing

## 📁 Project Structure

```
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/         # Route-based page components
│   │   ├── lib/           # Utilities and business logic
│   │   └── hooks/         # Custom React hooks
│   └── public/            # Static assets (hats, frames, icons)
├── server/                # Backend Express application
│   ├── routes.ts          # API route definitions
│   ├── storage.ts         # Data persistence layer
│   └── index.ts           # Server entry point
├── shared/                # Shared TypeScript schemas
└── attached_assets/       # Development assets and screenshots
```

## 🎨 Design System

### Color Palette
- **Primary**: #ff4a00 (P33ly Orange)
- **Background**: Linear gradient from #1a1a1a to #2d1810
- **Text**: White with transparency variants
- **Accents**: Blue (#0088ff), Green (#00ff00) for controls

### Typography
- **Font Family**: Outfit (Google Fonts)
- **Responsive Sizing**: clamp() functions for all screen sizes
- **Weight Scale**: 400 (regular) to 600 (semibold)

### Interactive Elements
- **Control Buttons**: 30px circular buttons with 15px radius
- **Touch Targets**: Minimum 44px for accessibility
- **Hover Effects**: Smooth transitions with scale and opacity changes

## 📱 Mobile Optimization

### Touch Interactions
- **120fps Throttling**: Ultra-smooth control responsiveness
- **Momentum Physics**: Natural movement with easing curves
- **Multi-touch Support**: Simultaneous hat editing operations
- **Gesture Recognition**: Pinch-to-zoom and rotation gestures

### Responsive Breakpoints
- **Mobile**: 320px - 768px (single column layout)
- **Tablet**: 768px - 1024px (adaptive grid)
- **Desktop**: 1024px+ (full feature layout)

## 🎯 Usage Guide

### Basic Workflow
1. **Upload Image**: Drag your profile picture or click to browse
2. **Select Hat**: Choose from 4 P33ly-themed hat options
3. **Pick Frame**: Select decorative frame or go frameless
4. **Customize**: Adjust hat size, rotation, and position
5. **Download**: Export as PNG with p33l_pfp.png filename

### Advanced Editing
1. **Control Modes**: Switch between Move, Resize, and Rotate
2. **Precision Adjustment**: Use sliders for exact positioning
3. **Animation Settings**: Enable rotating frames with custom speed
4. **Quality Options**: Choose output size and format

## 🔧 Configuration

### Environment Variables
```bash
NODE_ENV=development          # Environment mode
PORT=5000                    # Server port
DATABASE_URL=postgresql://... # Database connection (optional)
```

### Customization Options
- **Hat Assets**: Add new hats in `/client/public/` directory
- **Frame Assets**: Add custom frames with transparency
- **Color Scheme**: Modify CSS variables in `/client/src/index.css`
- **Branding**: Update logo and mascot assets

## 🚀 Deployment

### Replit Deployment
The application is optimized for Replit deployment:
- Automatic port detection and binding
- Environment variable support
- Hot reload in development
- Production build optimization

### Manual Deployment
```bash
# Build application
npm run build

# Deploy to your preferred hosting platform
# Static files in dist/public/
# Server bundle in dist/index.js
```

## 🧪 Testing

### Development Testing
- Real-time hot reload for immediate feedback
- Canvas rendering validation
- Mobile responsiveness testing
- Cross-browser compatibility

### Performance Optimization
- **Canvas Efficiency**: Optimized drawing operations
- **Memory Management**: Proper image disposal
- **Asset Loading**: Lazy loading of hat and frame images
- **Animation Smoothing**: 120fps throttling with momentum

## 🤝 Contributing

### Development Guidelines
1. Follow TypeScript strict mode requirements
2. Use Tailwind CSS for all styling
3. Maintain mobile-first responsive design
4. Follow accessibility best practices
5. Document all new features and changes

### Code Style
- **Formatting**: Prettier with 2-space indentation
- **Linting**: ESLint with React and TypeScript rules
- **Naming**: camelCase for variables, PascalCase for components
- **Files**: kebab-case for file names

## 📄 License

MIT License - see LICENSE file for details

## 🔗 Links

- **Live Demo**: [p33ly-pfp-editor.replit.app](https://p33ly-pfp-editor.replit.app)
- **Documentation**: [GitHub Wiki](https://github.com/yourusername/p33ly-pfp-editor/wiki)
- **Issues**: [GitHub Issues](https://github.com/yourusername/p33ly-pfp-editor/issues)
- **P33ly Community**: [Official Website](https://p33ly.com)

---

Made with ❤️ for the P33ly community