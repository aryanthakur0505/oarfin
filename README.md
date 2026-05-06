# 🌍 OARFIN - Disaster Management Platform

**Open-source Adaptive Real-time Framework for Intelligent Navigation**

A comprehensive disaster management system providing real-time navigation, safe spot identification, and emergency resource mapping during natural disasters.

[![React](https://img.shields.io/badge/React-19.0.0-blue.svg)](https://reactjs.org/)
[![Node.js](https://img.shields.io/badge/Node.js-Express-green.svg)](https://nodejs.org/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

## 🚀 Features

### 🗺️ Interactive Disaster Map
- Real-time visualization using **Leaflet.js** and **React-Leaflet**
- Dynamic disaster filtering (floods, earthquakes, fires, etc.)
- User-contributed safe spot marking and sharing
- 5km radius safe location identification (hospitals, shelters, police stations)

### 📰 Live Disaster News Aggregation
- Automated web scraping using **Playwright**
- Real-time news articles from multiple sources
- Reddit video integration for on-ground updates
- Cached responses for optimized performance

### 🤖 AI-Powered Assistance
- **Google Generative AI** integration for contextual disaster analysis
- **OpenAI API** chatbot for emergency guidance
- Context-aware recommendations based on disaster type and location

### 🔒 Security & Performance
- JWT authentication for secure access
- SQLite database for persistent data storage
- Node-cache for API response optimization
- CORS configuration for cross-origin requests

## 🛠️ Tech Stack

### Frontend
- **React 19** with Vite
- **Leaflet.js** for interactive maps
- **Tailwind CSS** for styling
- **Axios** for API communication

### Backend
- **Node.js** with **Express.js**
- **Playwright** for web scraping
- **SQLite3** for database
- **node-cache** for caching layer
- **Google Generative AI** & **OpenAI** APIs

### APIs & Services
- **Overpass API** for OpenStreetMap data
- **JWT** for authentication
- RESTful API architecture

## 📁 Project Structure

```
oarfin/
├── website/                 # React frontend
│   ├── src/
│   │   ├── App.jsx
│   │   ├── HomePage.jsx
│   │   ├── Dashboard.jsx
│   │   ├── DisasterMap.jsx
│   │   ├── NewsArticles.jsx
│   │   ├── RedditVideos.jsx
│   │   ├── DisasterFilter.jsx
│   │   └── SafeSpotMarker.jsx
│   └── package.json
│
├── server/                  # Node.js backend
│   ├── src/
│   │   ├── controllers/
│   │   │   └── scraperController.js
│   │   ├── services/
│   │   │   ├── overpassService.js
│   │   │   └── scraperService.js
│   │   └── routes/
│   │       └── scraper.js
│   ├── disaster_alert.db    # SQLite database
│   └── package.json
│
└── chapters/                # BTP Report LaTeX files
```

## 🚀 Getting Started

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn
- Git

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/vishisht-trivedi/Oarfin_DisasterManagement.git
cd Oarfin_DisasterManagement
```

2. **Setup Backend**
```bash
cd server
npm install
```

Create `.env` file in `server/` directory:
```env
PORT=5000
GOOGLE_AI_API_KEY=your_google_ai_key
OPENAI_API_KEY=your_openai_key
JWT_SECRET=your_jwt_secret
```

3. **Setup Frontend**
```bash
cd ../website
npm install
```

Create `.env` file in `website/` directory:
```env
VITE_API_URL=http://localhost:5000
```

### Running the Application

**Start Backend Server:**
```bash
cd server
npm run dev
```
Server runs on `http://localhost:5000`

**Start Frontend:**
```bash
cd website
npm run dev
```
Frontend runs on `http://localhost:5173`

## 🎯 Usage

1. **View Disaster Map**: Navigate to the homepage to see real-time disaster locations
2. **Filter by Disaster Type**: Use the filter panel to view specific disaster types
3. **Find Safe Spots**: Click on the map to identify nearby safe locations
4. **Read News**: Access aggregated disaster news and Reddit videos
5. **AI Assistance**: Use the chatbot for emergency guidance and recommendations

## 🔑 Key Features Explained

### Disaster Filtering
Filter disasters by type with real-time count updates:
- 🌊 Floods
- 🔥 Fires
- 🌪️ Tornadoes
- ⚡ Earthquakes
- 🌋 Volcanic Activity

### Safe Spot Identification
Automatically identifies safe locations within 5km radius:
- 🏥 Hospitals
- 🏠 Emergency Shelters
- 👮 Police Stations
- 🚒 Fire Stations

### Web Scraping Pipeline
- Automated news aggregation from multiple sources
- Reddit video scraping for real-time updates
- Cached responses to reduce API calls by 70%

## 📊 Performance Metrics

- **API Response Time**: Reduced by 70% with caching
- **Safe Location Query**: <2s for 5km radius search
- **Real-time Updates**: News refresh every 5 minutes
- **Map Rendering**: Optimized for 1000+ markers

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors

**Vishisht Trivedi**
- GitHub: [@vishisht-trivedi](https://github.com/vishisht-trivedi)
- Email: vishishttrivedi1050@gmail.com

## 🙏 Acknowledgments

- OpenStreetMap for geospatial data
- Google Generative AI for intelligent assistance
- The open-source community for amazing tools and libraries

## 📧 Contact

For questions or support, please open an issue or contact:
- Email: vishishttrivedi1050@gmail.com
- LinkedIn: [Your LinkedIn Profile]

---

**⭐ If you find this project useful, please consider giving it a star!**
