# AI Research Article Analyzer

A full-stack web application that analyzes research papers and articles using AI to extract summaries, key points, and keywords.

## Features

- **Multi-URL Analysis**: Analyze one or multiple articles simultaneously.
- **Content Extraction**: Automatically fetches and cleans article text from URLs.
- **AI Insights**: Powered by Gemini 3 to provide:
  - Title & Site Name
  - Executive Summary (5-7 lines)
  - Key Points (Bullet format)
  - Keywords
  - Main Conclusion
- **Clean UI**: Minimalist, professional design with loading states and error handling.

## Tech Stack

- **Frontend**: React 19, Vite, Tailwind CSS, Framer Motion, Lucide Icons.
- **Backend**: Node.js, Express (handles article scraping).
- **AI**: Google Gemini 3 API.
- **Scraping**: JSDOM + @mozilla/readability (standard for article extraction).

## Local Setup

1. **Clone the repository** (or download the files).
2. **Install dependencies**:
   ```bash
   npm install
   ```
3. **Set up Environment Variables**:
   Create a `.env` file in the root directory and add your Gemini API Key:
   ```env
   GEMINI_API_KEY=your_api_key_here
   ```
4. **Run the development server**:
   ```bash
   npm run dev
   ```
5. **Open the app**:
   Navigate to `http://localhost:3000` in your browser.

## Project Structure

- `server.ts`: Express backend for fetching and parsing article HTML.
- `src/App.tsx`: Main React frontend with AI integration.
- `src/types.ts`: Shared TypeScript interfaces.
- `src/lib/utils.ts`: Utility functions for styling.
- `vite.config.ts`: Configuration for Vite and environment variables.
