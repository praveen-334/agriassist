# AgriAssist - Smart Farming Solutions

A comprehensive agricultural technology platform that empowers farmers with AI-powered tools for crop disease diagnosis, market analysis, and government scheme navigation.

## Features

- **Crop Disease Diagnosis**: Upload crop photos for AI-powered disease detection and treatment recommendations
- **Real-time Market Analysis**: Get current crop prices and market insights
- **Government Schemes**: Browse and apply for agricultural subsidies and programs
- **Voice Interface**: Voice commands for hands-free operation
- **Mobile-first Design**: Optimized for smartphones and tablets

## Prerequisites

- Node.js 18+ installed on your computer
- A Gemini API key from Google AI Studio (free)

## Local Installation

### 1. Download the Code

```bash
# If you have git installed
git clone <your-repo-url>
cd agriassist

# Or download and extract the ZIP file from Replit
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Set Up Environment Variables

Create a `.env` file in the root directory:

```bash
# Create .env file
touch .env
```

Add your Gemini API key to the `.env` file:

```
GEMINI_API_KEY=your_gemini_api_key_here
```

### 4. Run the Application

```bash
# Start both frontend and backend
npm run dev
```

The app will be available at: `http://localhost:5000`

## Getting Your Gemini API Key

1. Go to [Google AI Studio](https://aistudio.google.com/)
2. Sign in with your Google account
3. Click "Get API Key" and create a new project
4. Copy the generated API key
5. Add it to your `.env` file

## Project Structure

```
agriassist/
├── client/                 # React frontend
│   ├── src/
│   │   ├── components/     # UI components
│   │   ├── hooks/         # Custom React hooks
│   │   ├── lib/           # Utility functions
│   │   └── pages/         # Page components
│   └── index.html
├── server/                # Express backend
│   ├── data/             # Sample data
│   ├── services/         # AI services
│   └── routes.ts         # API routes
├── shared/               # Shared types and schemas
└── package.json
```

## Available Scripts

```bash
# Start development server
npm run dev

# Build for production
npm run build

# Start production server
npm start

# Database migrations
npm run db:migrate

# Generate database types
npm run db:generate
```

## Usage

### Disease Diagnosis
1. Click "Diagnose Now" on the main dashboard
2. Take a photo or upload an image of your crop
3. Wait for AI analysis
4. Review disease detection results and treatment recommendations

### Market Analysis
1. Click "Check Prices" to view current crop prices
2. View market trends and price changes
3. Read AI-generated market insights

### Government Schemes
1. Click "View Schemes" to browse available programs
2. Filter by category (subsidies, insurance, training)
3. View eligibility criteria and application processes

### Voice Commands
1. Click "Voice Mode" in the header
2. Say commands like:
   - "Diagnose crop"
   - "Check market prices"
   - "Show government schemes"

## Mobile Usage

The app is optimized for mobile devices:
- Responsive design works on all screen sizes
- Camera integration for crop photos
- Touch-friendly interface
- Voice commands for hands-free operation

## Troubleshooting

### Common Issues

**App won't start:**
- Make sure Node.js 18+ is installed
- Run `npm install` to install dependencies
- Check that port 5000 is available

**Disease diagnosis not working:**
- Verify your Gemini API key is correct
- Check internet connection
- Ensure image files are in supported formats (JPG, PNG)

**Voice commands not working:**
- Use Chrome, Firefox, or Safari browsers
- Allow microphone permissions
- Ensure you're on HTTPS or localhost

### Environment Variables

Required environment variables:
- `GEMINI_API_KEY`: Your Google AI Studio API key

Optional environment variables:
- `PORT`: Server port (default: 5000)
- `NODE_ENV`: Environment (development/production)

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is licensed under the MIT License.

## Support

For technical support or questions:
- Email: support@agriassist.com
- Phone: 1800-123-4567
- Available 24/7

## Technologies Used

- **Frontend**: React, TypeScript, Tailwind CSS
- **Backend**: Node.js, Express
- **AI**: Google Gemini API
- **Database**: PostgreSQL (Neon)
- **Build Tool**: Vite
- **UI Components**: Radix UI, shadcn/ui