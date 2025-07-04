# Download AgriAssist - Complete Setup Package

## Method 1: Download from Replit (Recommended)

1. **In your Replit project, click the 3 dots menu** (⋮) in the top right
2. **Select "Download as zip"**
3. **Extract the zip file** to your desired location
4. **Follow the setup steps below**

## Method 2: Manual File Copy

Copy all these files and folders to your local computer:

### Required Files:
```
📁 agriassist/
├── 📁 client/
│   ├── 📁 src/
│   │   ├── 📁 components/
│   │   ├── 📁 hooks/
│   │   ├── 📁 lib/
│   │   └── 📁 pages/
│   └── 📄 index.html
├── 📁 server/
│   ├── 📁 data/
│   ├── 📁 services/
│   ├── 📄 index.ts
│   ├── 📄 routes.ts
│   ├── 📄 storage.ts
│   └── 📄 vite.ts
├── 📁 shared/
│   └── 📄 schema.ts
├── 📄 package.json
├── 📄 vite.config.ts
├── 📄 tailwind.config.ts
├── 📄 tsconfig.json
├── 📄 drizzle.config.ts
├── 📄 components.json
└── 📄 postcss.config.js
```

## Setup Instructions (After Download)

### 1. Install Node.js
- Download Node.js 18+ from https://nodejs.org/
- Install and verify: `node --version`

### 2. Open Terminal/Command Prompt
```bash
cd path/to/your/agriassist-folder
```

### 3. Install Dependencies
```bash
npm install
```

### 4. Create Environment File
Create a file named `.env` in the root folder with:
```
GEMINI_API_KEY=your_api_key_here
```

### 5. Get Your API Key
1. Go to https://aistudio.google.com/
2. Sign in with Google account
3. Click "Get API Key"
4. Copy the key and paste it in your `.env` file

### 6. Start the App
```bash
npm run dev
```

Open your browser to: http://localhost:5000

## What You'll Get

✅ **Complete Agricultural App** with:
- AI crop disease diagnosis
- Real-time market prices
- Government scheme information
- Voice commands
- Mobile-responsive design
- Camera integration

✅ **Works Offline** for basic features
✅ **Production Ready** - can be deployed anywhere
✅ **Fully Customizable** - modify as needed

## Troubleshooting

### Common Issues:
- **Port 5000 busy**: Change PORT in `.env` file
- **API not working**: Check your Gemini API key
- **Dependencies error**: Delete `node_modules` and run `npm install`
- **Camera not working**: Use Chrome/Firefox and allow permissions

### System Requirements:
- Node.js 18+
- Modern web browser
- Internet connection (for AI features)
- Camera access (for crop photos)

## Need Help?

The app is designed to work immediately after following these steps. If you encounter issues:
1. Check that all files are copied correctly
2. Verify your API key is valid
3. Make sure port 5000 is available
4. Check browser console for error messages

Your AgriAssist app will be ready to help farmers diagnose crop diseases, check market prices, and navigate government schemes!