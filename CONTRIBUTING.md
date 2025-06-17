# Contributing to P33ly PFP Editor

We welcome contributions to the P33ly PFP Editor project! This guide will help you get started.

## Development Setup

1. **Fork and Clone**
   ```bash
   git clone https://github.com/yourusername/p33ly-pfp-editor.git
   cd p33ly-pfp-editor
   ```

2. **Install Dependencies**
   ```bash
   npm install
   ```

3. **Start Development Server**
   ```bash
   npm run dev
   ```

## Code Standards

### TypeScript
- Use strict TypeScript with proper typing
- Avoid `any` types when possible
- Use interfaces for component props

### React Components
- Use functional components with hooks
- Follow the existing component structure
- Implement proper error boundaries

### Styling
- Use Tailwind CSS for styling
- Follow mobile-first responsive design
- Use CSS variables for theming

### Code Formatting
- Use consistent indentation (2 spaces)
- Follow ESLint rules
- Use meaningful variable names

## Project Structure

```
client/src/
├── components/     # Reusable UI components
├── lib/           # Utility functions and canvas operations
├── pages/         # Main application pages
└── hooks/         # Custom React hooks

server/
├── index.ts       # Server setup and middleware
├── routes.ts      # API endpoint definitions
└── storage.ts     # Data persistence layer
```

## Making Changes

1. **Create a Feature Branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. **Make Your Changes**
   - Write clean, documented code
   - Test on both desktop and mobile
   - Ensure responsive design works

3. **Test Your Changes**
   ```bash
   npm run build
   npm run check
   ```

4. **Commit Changes**
   ```bash
   git add .
   git commit -m "feat: add your feature description"
   ```

5. **Push and Create PR**
   ```bash
   git push origin feature/your-feature-name
   ```

## Guidelines

### Canvas Operations
- Test image processing with various file types
- Ensure performance on mobile devices
- Validate touch event handling

### Mobile Responsiveness
- Test on actual mobile devices
- Verify touch targets are at least 44px
- Check text readability at all screen sizes

### Performance
- Optimize canvas rendering operations
- Minimize re-renders in React components
- Test with large image files

## Pull Request Process

1. Update README.md if needed
2. Ensure all tests pass
3. Update documentation for new features
4. Request review from maintainers

## Bug Reports

When reporting bugs, include:
- Browser and device information
- Steps to reproduce
- Expected vs actual behavior
- Screenshots if applicable

## Feature Requests

For new features:
- Describe the use case
- Explain the expected behavior
- Consider mobile implementation
- Check existing issues first

## Questions?

Feel free to open an issue for any questions about contributing.