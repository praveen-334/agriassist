# AgriAssist - Local Setup Guide

## Quick Start

1. **Download all files** from your Replit project
2. **Install Node.js 18+** from https://nodejs.org/
3. **Get your Gemini API key** from https://aistudio.google.com/
4. **Run the commands below**

## Step-by-Step Setup

### 1. Create Project Directory
```bash
mkdir agriassist
cd agriassist
```

### 2. Copy All Files
Copy all files from your Replit project to this directory, maintaining the same folder structure:

```
agriassist/
├── client/
│   ├── src/
│   │   ├── components/
│   │   ├── hooks/
│   │   ├── lib/
│   │   └── pages/
│   └── index.html
├── server/
│   ├── data/
│   ├── services/
│   └── (all server files)
├── shared/
├── package.json
└── (all other files)
```

### 3. Install Dependencies
```bash
npm install
```

### 4. Set Up Environment Variables
Create a `.env` file in the root directory:
```bash
GEMINI_API_KEY=your_api_key_here
PORT=5000
NODE_ENV=development
```

### 5. Start the Application
```bash
npm run dev
```

Your app will be available at: http://localhost:5000

## Commands Reference

```bash
# Development (starts both frontend and backend)
npm run dev

# Build for production
npm run build

# Start production server
npm start

# Preview production build
npm run preview
```

## Troubleshooting

### Port Already in Use
If port 5000 is busy, change it in your `.env` file:
```
PORT=3000
```

### API Key Issues
- Make sure your Gemini API key is correct
- Check that the `.env` file is in the root directory
- Restart the server after adding the API key

### Dependencies Issues
```bash
# Clear cache and reinstall
rm -rf node_modules package-lock.json
npm install
```

### Browser Issues
- Use Chrome, Firefox, or Safari for best compatibility
- Allow camera and microphone permissions for full functionality
- Clear browser cache if experiencing issues

## Features That Work Locally

✅ **Crop Disease Diagnosis** - Upload photos for AI analysis
✅ **Market Price Analysis** - Real-time crop pricing
✅ **Government Schemes** - Browse agricultural programs
✅ **Voice Commands** - Hands-free operation
✅ **Mobile Responsive** - Works on all devices
✅ **Camera Integration** - Take photos directly in browser

## Production Deployment

### Option 1: Manual Deploy
```bash
# Build the app
npm run build

# Upload dist/ folder to your hosting service
# Start with: node dist/server.js
```

### Option 2: Use Replit Deploy
Simply click the "Deploy" button in Replit for automatic deployment.

## System Requirements

- **Node.js**: 18.0 or higher
- **RAM**: 512MB minimum
- **Storage**: 100MB for app files
- **Internet**: Required for AI features

## File Structure Explained

```
├── client/                 # React frontend
│   ├── src/components/     # UI components
│   ├── src/hooks/         # Custom hooks
│   ├── src/lib/           # Utilities
│   └── src/pages/         # Page components
├── server/                # Express backend
│   ├── data/             # Sample data
│   ├── services/         # AI integration
│   └── routes.ts         # API endpoints
├── shared/               # Shared TypeScript types
├── package.json          # Dependencies
└── .env                  # Environment variables
```

## Important Notes

- The app needs internet connection for AI features
- Camera access required for crop photo capture
- Microphone access needed for voice commands
- Works best on modern browsers (Chrome, Firefox, Safari)
- Mobile-optimized for farmers in the field

## Getting Help

If you encounter issues:
1. Check the troubleshooting section above
2. Verify all files are copied correctly
3. Make sure your API key is valid
4. Check browser console for error messages

The app is designed to work offline for basic features, but AI diagnosis requires internet connectivity.