# 🏛️ Parliament Watch

**Making Canadian Politics Accessible and Transparent**

Parliament Watch is a comprehensive web platform that brings Canadian federal politics to your fingertips. Get AI-analyzed news from multiple perspectives, track legislation in plain language, explore MP profiles, and ask questions to an intelligent parliamentary chatbot — all in one place.

## 🌟 Features

### 📰 **Bias-Aware News Aggregation**
- Aggregates political news from multiple Canadian sources across the political spectrum
- AI-powered analysis showing how different perspectives cover the same story
- Side-by-side comparison of left-leaning, centrist, and right-leaning viewpoints
- Highlights common ground and unique emphasis from each political perspective
- Clean, modern interface with featured stories and topic cards

### 📜 **Federal Legislation Tracker**
- Plain-language summaries of Canadian bills and legislation
- Real-time status tracking from introduction through Royal Assent
- Filter by status: All Bills, Passed, or Pending
- Detailed voting records with party-by-party breakdowns
- Search by bill number, title, or content
- Direct links to official OpenParliament sources

### 👥 **MPs Directory**
- Searchable directory of all Canadian Members of Parliament
- Filter by party, province, riding, or name
- Official photos and contact information
- Detailed voting records and parliamentary participation
- Recent debate contributions and speeches
- Party affiliation with color-coded badges

### 🤖 **AI Parliamentary Assistant**
- Intelligent chatbot powered by Claude
- Answers questions about bills, MPs, voting records, and parliamentary procedures
- Grounded in real-time data from OpenParliament API
- Multi-turn conversations with context awareness
- Professional, informative tone with source citations

---

## 🚀 Quick Start

### Prerequisites

- **Node.js** 18+ and npm
- **Supabase** account (free tier works)
- **Claude API key** for Claude

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/sbalagan22/Cluade-Hackahton-COMP.git
   cd Cluade-Hackahton-COMP
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**

   Create a `.env` file in the root directory:
   ```env
   VITE_SUPABASE_URL=your_supabase_project_url
   VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
   VITE_CLAUDE_API_KEY=your_claude_api_key
   ```

   **Where to find these:**
   - **Supabase**: Dashboard → Project Settings → API
   - **Claude API**: [Claude API](https://claude.ai/)

4. **Set up the database**

   Run the SQL schema in your Supabase SQL Editor:
   ```bash
   cat supabase_schema.sql
   ```
   Then paste and execute in Supabase Dashboard → SQL Editor

5. **Run the development server**
   ```bash
   npm run dev
   ```

6. **Open your browser**
   
   Navigate to `http://localhost:5173`

---

## 🛠️ Technology Stack

### **Frontend**
- **React 18.2** - UI framework
- **Vite 5.0** - Build tool and dev server
- **React Router 6.20** - Client-side routing
- **TailwindCSS 3.3** - Utility-first CSS framework
- **TanStack React Query 5.0** - Data fetching and caching
- **Radix UI** - Accessible component primitives
- **Lucide React** - Icon library
- **date-fns** - Date formatting

### **Backend & Services**
- **Supabase** - PostgreSQL database and edge functions
- **Claude 3.5 Haiku** - AI language model
- **OpenParliament.ca API** - Canadian parliamentary data

### **Development Tools**
- **ESLint** - Code linting
- **PostCSS** - CSS processing
- **Autoprefixer** - CSS vendor prefixing

---

## 🎨 Key Components

### News Feed
- **Aggregation**: Fetches RSS feeds from CBC, CTV, Global News, National Post, Toronto Star
- **AI Analysis**: Groups articles by topic and analyzes political bias
- **Visualization**: Color-coded bias distribution bars showing source breakdown

### Bills Tracker
- **Data Source**: OpenParliament API for real-time bill information
- **Filtering**: Status-based filtering (Passed vs Pending)
- **Search**: Full-text search across bill numbers, titles, and summaries
- **Details**: Modal view with voting records and party positions

### MPs Directory
- **Comprehensive**: All 338 current Members of Parliament
- **Search**: Multi-field search (name, riding, party, province)
- **Profiles**: Detailed modals with voting history and debate participation
- **Party Filtering**: Quick filters for major political parties

### AI Chatbot
- **Intent Classification**: Detects whether questions are about bills, MPs, or votes
- **Data Grounding**: Fetches real data from OpenParliament API
- **Context Awareness**: Maintains conversation history
- **Source Attribution**: Provides links to official sources

---

## 📊 Data Sources

### OpenParliament.ca API
Official Canadian parliamentary data including:
- Current session bills and legislation
- MP information and profiles
- Voting records and results
- Debate transcripts (Hansard)
- Committee information

### RSS News Feeds
Political news aggregated from:
- **CBC News** (Left-leaning)
- **Toronto Star** (Left-leaning)
- **CTV News** (Centre)
- **Global News** (Centre)
- **National Post** (Right-leaning)



<div align="center">

Made with ❤️ for Canadian democracy

</div>

