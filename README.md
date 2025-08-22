# YOGAAROGYA Frontend

## Overview
React TypeScript application providing personalized yoga recommendations based on health assessments.

## Features
- User authentication and profiles
- Health condition assessment
- Personalized yoga pose recommendations
- Video tutorials for each pose
- Session timer and progress tracking
- User feedback system
- Real-time testimonials
- Dark/Light theme toggle
- Responsive design

## Tech Stack
- **Framework**: React 18 with TypeScript
- **Build Tool**: Vite
- **Styling**: Tailwind CSS
- **Icons**: Lucide React
- **Charts**: Chart.js with react-chartjs-2
- **Routing**: React Router DOM
- **State Management**: React Context
- **Backend**: Supabase (BaaS)

## Project Structure
```
src/
├── components/          # Reusable UI components
│   ├── Layout.tsx      # Main layout wrapper
��   └── UserCounter.tsx # User count display
├── context/            # React contexts
│   ├── AuthContext.tsx # Authentication state
│   └── ThemeContext.tsx # Theme management
├── lib/                # Utilities and configurations
│   └── supabase.ts     # Supabase client setup
├── pages/              # Page components
│   ├── Dashboard.tsx   # User dashboard
│   ├── Feedback.tsx    # Feedback form
│   ├── HealthAssessment.tsx # Health condition form
│   ├── Home.tsx        # Landing page
│   ├── Login.tsx       # Login form
│   ├── SignUp.tsx      # Registration form
│   ├── YogaRecommendations.tsx # Pose recommendations
│   └── YogaSession.tsx # Session timer
├── types/              # TypeScript type definitions
│   └── supabase.ts     # Database type definitions
├── App.tsx             # Main app component
├── main.tsx           # App entry point
└── index.css          # Global styles
```

## Setup Instructions

### Prerequisites
- Node.js 18+ 
- npm or yarn
- Supabase account and project

### Installation
1. Clone the repository
```bash
git clone https://github.com/shrutishitole20/yogaarogya.git
cd yogaarogya/frontend
```

2. Install dependencies
```bash
npm install --legacy-peer-deps
```

3. Set up environment variables
```bash
cp .env.example .env
```

4. Update `.env` with your Supabase credentials:
```env
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```

5. Start development server
```bash
npm run dev
```

## Available Scripts
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

## Environment Variables
- `VITE_SUPABASE_URL` - Your Supabase project URL
- `VITE_SUPABASE_ANON_KEY` - Your Supabase anonymous key

## Deployment

### Vercel (Recommended)
1. Connect your GitHub repository to Vercel
2. Add environment variables in Vercel dashboard
3. Deploy automatically on git push

### Netlify
1. Build the project: `npm run build`
2. Deploy the `dist` folder to Netlify
3. Add environment variables in Netlify dashboard

### Manual Deployment
1. Build: `npm run build`
2. Serve the `dist` folder with any static hosting service

## Features in Detail

### Authentication
- Email/password registration and login
- Profile creation with health information
- Protected routes for authenticated users

### Health Assessment
- Comprehensive health condition questionnaire
- 15+ health conditions covered
- Personalized recommendations based on responses

### Yoga Recommendations
- Dynamic pose suggestions based on health assessment
- Video tutorials for each pose
- Difficulty levels and categories
- Session tracking and progress monitoring

### Session Timer
- Customizable workout timers
- Progress tracking with visual indicators
- Session history and statistics

### User Experience
- Responsive design for all devices
- Dark/light theme support
- Smooth animations and transitions
- Real-time feedback display

## Contributing
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License
MIT License - see LICENSE file for details
