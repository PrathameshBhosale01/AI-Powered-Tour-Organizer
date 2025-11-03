# 🌍 AI-Powered Tour Organizer

<div align="center">

![AI Tour Organizer Banner](https://img.shields.io/badge/AI-Powered-blue?style=for-the-badge&logo=openai)
![Next.js](https://img.shields.io/badge/Next.js-15.1.4-black?style=for-the-badge&logo=next.js)
![Firebase](https://img.shields.io/badge/Firebase-Integrated-orange?style=for-the-badge&logo=firebase)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

**An intelligent web application that revolutionizes travel planning through AI-powered personalization and real-time data integration.**

[Live Demo](#) • [Report Bug](https://github.com/PrathameshBhosale01/AI-Powered-Tour-Organizer/issues) • [Request Feature](https://github.com/PrathameshBhosale01/AI-Powered-Tour-Organizer/issues)

</div>

---

## 📋 Table of Contents

- [About The Project](#-about-the-project)
- [Key Features](#-key-features)
- [Tech Stack](#-tech-stack)
- [Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Environment Variables](#environment-variables)
- [Usage](#-usage)
- [Project Structure](#-project-structure)
- [API Integrations](#-api-integrations)
- [Screenshots](#-screenshots)
- [Roadmap](#-roadmap)
- [Contributing](#-contributing)
- [License](#-license)
- [Contact](#-contact)
- [Acknowledgments](#-acknowledgments)

---

## 🎯 About The Project

The **AI-Powered Tour Organizer** is a cutting-edge web application designed to transform the way travelers plan their journeys. Built with modern technologies and powered by Generative AI, it eliminates the complexity of traditional travel planning by automating itinerary generation, integrating real-time data, and providing personalized recommendations.

### 🌟 Why This Project?

Traditional travel planning is:
- ⏰ **Time-consuming** - Juggling multiple platforms for flights, hotels, and activities
- 🔄 **Fragmented** - Scattered information across different websites
- 📊 **Static** - Limited personalization and outdated recommendations
- 🤯 **Overwhelming** - Too many options without intelligent filtering

**Our Solution** provides a unified, intelligent platform that understands your preferences, budget, and constraints to deliver optimized, personalized travel experiences.

### 🎓 Academic Project

This project was developed as part of the **Major Project I** for Bachelor of Engineering (Computer Engineering) at **Terna Engineering College, University of Mumbai** (2025-2026).

**Developer:** Prathamesh Bhosale (TU3F2223004)

**Guide:** Prof. Varsha Pande

---

## ✨ Key Features

### 🤖 AI-Powered Intelligence
- **Smart Itinerary Generation** - Leverages Google Gemini AI to create personalized travel plans
- **Natural Language Processing** - Understands user preferences in plain language
- **Adaptive Recommendations** - Learns from user interactions for better suggestions

### 🗺️ Real-Time Integration
- **Live Weather Updates** - Current weather conditions for destinations
- **Interactive Maps** - Google Maps integration for location visualization
- **Dynamic Pricing** - Real-time flight and hotel price updates via web scraping

### 👤 User Experience
- **Seamless Authentication** - Firebase Auth with Google OAuth support
- **Profile Management** - Personalized user dashboards and trip history
- **Dark/Light Mode** - Theme switching for comfortable viewing
- **Multi-Language Support** - Accessible to global users

### 🛠️ Travel Tools
- **Expense Tracker** - Monitor and manage travel budgets
- **Currency Converter** - Real-time exchange rates
- **Trip Scheduler** - Organize daily activities and timelines
- **OpenTripMap Integration** - Discover tourist attractions and POIs

### 📝 Community Features
- **Blog/Zone** - Share travel experiences and stories
- **Comments System** - Engage with fellow travelers
- **Image Uploads** - Cloudinary-powered media management
- **Trip Reviews** - Rate and review destinations

### 🔐 Security & Performance
- **Encrypted Data** - Secure storage with Firebase Firestore
- **HTTPS Protocol** - Safe data transmission
- **Responsive Design** - Optimized for all devices
- **Fast Loading** - Next.js App Router for optimal performance

---

## 🛠️ Tech Stack

### Core Technologies

| Category | Technology | Version | Purpose |
|----------|-----------|---------|---------|
| **Framework** | Next.js | 15.1.4 | React framework with App Router |
| **UI Library** | React | 19.0.0 | Component-based UI development |
| **Styling** | TailwindCSS | 3.4.1 | Utility-first CSS framework |
| **Components** | shadcn/ui | Latest | Pre-built accessible components |
| **Language** | JavaScript | ES6+ | Primary programming language |

### Backend & Database

| Service | Technology | Purpose |
|---------|-----------|---------|
| **Database** | Firebase Firestore | NoSQL cloud database for trips, blogs, users |
| **Authentication** | Firebase Auth | User authentication with Google OAuth |
| **Storage** | Firebase Storage | Cloud storage for user data |
| **Real-time Sync** | Firebase Realtime DB | Live data synchronization |

### AI & External APIs

| API | Provider | Integration | Purpose |
|-----|----------|-------------|---------|
| **Generative AI** | Google Gemini | `lib/AI_Model.js` | Personalized itinerary generation |
| **Image Upload** | Cloudinary | `/api/upload` | Image optimization and CDN delivery |
| **Tourist POIs** | OpenTripMap | Utility integration | Discover attractions and landmarks |
| **Weather Data** | Weather API | Real-time fetch | Live weather forecasts |
| **Currency** | Exchange Rate API | Conversion utility | Real-time currency conversion |
| **Maps** | Google Maps | Embedded integration | Location visualization |

### Development Tools

| Tool | Purpose |
|------|---------|
| ![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white) | Version control and collaboration |
| ![npm](https://img.shields.io/badge/npm-CB3837?logo=npm&logoColor=white) | Package management |
| ![VS Code](https://img.shields.io/badge/VS_Code-007ACC?logo=visual-studio-code&logoColor=white) | Code editor |
| ![Postman](https://img.shields.io/badge/Postman-FF6C37?logo=postman&logoColor=white) | API testing |

---

## 🚀 Getting Started

### Prerequisites

Ensure you have the following installed:

- **Node.js** (v18.0.0 or higher)
- **npm** / **pnpm** / **yarn** / **bun** (package manager)
- **Git** (for cloning the repository)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/PrathameshBhosale01/AI-Powered-Tour-Organizer.git
   cd AI-Powered-Tour-Organizer
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   pnpm install
   # or
   yarn install
   # or
   bun install
   ```

3. **Set up environment variables**
   
   Create a `.env.local` file in the root directory (see [Environment Variables](#environment-variables))

4. **Run the development server**
   ```bash
   npm run dev
   # or
   pnpm dev
   # or
   yarn dev
   # or
   bun dev
   ```

5. **Open your browser**
   
   Navigate to [http://localhost:3000](http://localhost:3000)

### Environment Variables

Create a `.env.local` file in the root directory with the following variables:

```env
# Firebase Configuration
NEXT_PUBLIC_FIREBASE_API_KEY=your_firebase_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_firebase_auth_domain
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_firebase_project_id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_firebase_storage_bucket
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_firebase_messaging_sender_id
NEXT_PUBLIC_FIREBASE_APP_ID=your_firebase_app_id

# Google Generative AI (Gemini)
NEXT_PUBLIC_GEMINI_API_KEY=your_gemini_api_key

# Cloudinary (Image Uploads)
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
NEXT_PUBLIC_CLOUDINARY_UPLOAD_PRESET=your_cloudinary_upload_preset

# OpenTripMap API
NEXT_PUBLIC_OPENTRIPMAP_API_KEY=your_opentripmap_api_key

# Weather API (Optional)
NEXT_PUBLIC_WEATHER_API_KEY=your_weather_api_key

# Google Maps API (Optional)
NEXT_PUBLIC_GOOGLE_MAPS_API_KEY=your_google_maps_api_key
```

#### How to Obtain API Keys:

1. **Firebase**: Visit [Firebase Console](https://console.firebase.google.com/) → Create Project → Get Config
2. **Google Gemini AI**: Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
3. **Cloudinary**: Sign up at [Cloudinary](https://cloudinary.com/)
4. **OpenTripMap**: Register at [OpenTripMap](https://opentripmap.io/product)
5. **Weather API**: Get key from [OpenWeatherMap](https://openweathermap.org/api)
6. **Google Maps**: Enable at [Google Cloud Console](https://console.cloud.google.com/)

---

## 💡 Usage

### Creating Your First Trip

1. **Sign Up / Log In**
   - Use Google OAuth or email authentication
   - Complete your profile setup

2. **Create New Trip**
   - Navigate to "Create Trip" page
   - Enter destination, dates, budget, and preferences
   - Click "Generate Itinerary"

3. **AI-Generated Itinerary**
   - Review the AI-generated day-by-day plan
   - Customize activities, timings, and locations
   - Save to your dashboard

4. **Manage Your Trips**
   - View all saved trips on your dashboard
   - Edit details or delete trips
   - Share itineraries with friends

5. **Explore Community**
   - Read travel blogs and experiences
   - Post your own stories with images
   - Comment and engage with other travelers

### Using Travel Tools

- **Currency Converter**: Real-time exchange rates for budgeting
- **Weather Forecast**: 7-day weather predictions for destinations
- **Expense Tracker**: Log and categorize travel expenses
- **Map Explorer**: Discover nearby attractions and points of interest

---

## 📁 Project Structure

```
AI-Powered-Tour-Organizer/
├── app/                          # Next.js App Router pages
│   ├── (auth)/                   # Authentication pages
│   ├── blog/                     # Blog & Zone features
│   ├── create-trip/              # Trip creation interface
│   ├── dashboard/                # User dashboard
│   ├── profile/                  # User profile management
│   ├── view-trip/                # Trip detail viewer
│   └── layout.js                 # Root layout component
├── components/                   # Reusable React components
│   ├── ui/                       # shadcn/ui components
│   ├── custom/                   # Custom components
│   │   ├── Header.jsx
│   │   ├── Footer.jsx
│   │   └── ...
├── lib/                          # Utility libraries
│   ├── AI_Model.js               # Google Gemini AI integration
│   ├── firebase.js               # Firebase configuration
│   └── utils.js                  # Helper functions
├── public/                       # Static assets
│   ├── images/
│   └── icons/
├── styles/                       # Global styles
│   └── globals.css
├── .env.local                    # Environment variables (create this)
├── next.config.js                # Next.js configuration
├── tailwind.config.js            # Tailwind CSS configuration
├── package.json                  # Dependencies
└── README.md                     # Project documentation
```

---

## 🔌 API Integrations

### Google Generative AI (Gemini)
- **Purpose**: Generate personalized travel itineraries
- **File**: `lib/AI_Model.js`
- **Features**: Natural language understanding, context-aware recommendations

### Firebase Services
- **Firestore Database**: Store trips, blogs, user data
- **Firebase Auth**: User authentication and authorization
- **Cloud Storage**: Image and media storage

### Cloudinary
- **Purpose**: Image upload and optimization
- **Route**: `/api/upload` (API route)
- **Features**: Auto-optimization, CDN delivery, fallback to data URLs

### OpenTripMap
- **Purpose**: Discover tourist attractions and POIs
- **Features**: Location-based recommendations, attraction details

### Weather API
- **Purpose**: Real-time weather forecasts
- **Features**: Current conditions, 7-day forecasts, weather alerts

### Currency Converter API
- **Purpose**: Real-time exchange rates
- **Features**: Multi-currency support, historical data

---

## 📸 Screenshots

### Landing Page

<img width="855" height="780" alt="Screenshot 2025-11-03 133805" src="https://github.com/user-attachments/assets/e1e86611-9269-407f-a9e1-392d5803467d" />
<img width="867" height="830" alt="Screenshot 2025-11-03 133216" src="https://github.com/user-attachments/assets/b6f0a402-4f45-4256-9083-cd1df0e21619" />

*Modern, engaging landing page with call-to-action*

### Dashboard

<img width="1914" height="866" alt="Screenshot 2025-11-03 134520" src="https://github.com/user-attachments/assets/969a9243-4062-4162-b67e-881aa0895202" />

*User dashboard showing saved trips and quick actions*

---

## 🗺️ Roadmap

### Phase 1: Core Features ✅
- [x] User authentication and profile management
- [x] AI-powered itinerary generation
- [x] Trip CRUD operations
- [x] Blog and community features
- [x] Image upload functionality

### Phase 2: Enhanced Features 🚧
- [ ] Voice-based trip planning
- [ ] Direct booking integration (flights, hotels)
- [ ] Social sharing capabilities
- [ ] Mobile app (React Native)
- [ ] AR/VR destination previews

### Phase 3: Advanced AI 🔮
- [ ] Predictive travel demand forecasting
- [ ] Sentiment analysis for reviews
- [ ] Multi-user collaborative trip planning
- [ ] Real-time itinerary adjustment based on events
- [ ] AI travel companion chatbot

### Phase 4: Business Features 💼
- [ ] Travel agency partnerships
- [ ] Monetization through affiliates
- [ ] Premium subscription plans
- [ ] Analytics dashboard for users
- [ ] API for third-party integrations

---

## 🤝 Contributing

Contributions make the open-source community an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**!

### How to Contribute

1. **Fork the Project**
2. **Create your Feature Branch**
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. **Commit your Changes**
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```
4. **Push to the Branch**
   ```bash
   git push origin feature/AmazingFeature
   ```
5. **Open a Pull Request**

### Development Guidelines

- Follow the existing code style and conventions
- Write meaningful commit messages
- Update documentation for new features
- Test thoroughly before submitting PR
- Keep PRs focused and atomic

---

## 📄 License

Distributed under the MIT License. See `LICENSE` file for more information.

---

## 📧 Contact

**Prathamesh Bhosale**

- GitHub: [@PrathameshBhosale01](https://github.com/PrathameshBhosale01)
- Project Link: [AI-Powered Tour Organizer](https://github.com/PrathameshBhosale01/AI-Powered-Tour-Organizer)

---

## 🙏 Acknowledgments

I extend my sincere gratitude to:

- **Google** - For Gemini AI and Firebase services
- **Vercel** - For Next.js framework and hosting platform
- **Cloudinary** - For image management solutions
- **shadcn/ui** - For beautiful UI components
- **The Open Source Community** - For amazing libraries and tools

---

## 📊 Project Statistics

![GitHub stars](https://img.shields.io/github/stars/PrathameshBhosale01/AI-Powered-Tour-Organizer?style=social)
![GitHub forks](https://img.shields.io/github/forks/PrathameshBhosale01/AI-Powered-Tour-Organizer?style=social)
![GitHub issues](https://img.shields.io/github/issues/PrathameshBhosale01/AI-Powered-Tour-Organizer)
![GitHub pull requests](https://img.shields.io/github/issues-pr/PrathameshBhosale01/AI-Powered-Tour-Organizer)

---

<div align="center">

**Developed by Prathamesh Bhosale**

*Transforming Travel Planning, One Itinerary at a Time*

[⬆ Back to Top](#-ai-powered-tour-organizer)

</div>
