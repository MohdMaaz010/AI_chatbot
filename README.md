# EcoChoice AI - Eco-Friendly Product Recommender

![EcoChoice AI Banner](https://images.unsplash.com/photo-1542601906990-b4d3fb778b09?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80)

## Overview

EcoChoice AI is an interactive web application that uses artificial intelligence to recommend eco-friendly and sustainable products based on user preferences and needs. The app features a smart chatbot powered by Google's Gemini AI that provides personalized sustainability advice and product recommendations.

## Key Features

- **AI-Powered Recommendations**: Get personalized eco-friendly product suggestions through natural conversation
- **Category Exploration**: Browse different sustainability categories with specialized AI recommendations
- **Educational Content**: Learn about sustainable alternatives and their environmental benefits
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Markdown Formatting**: Clean and readable AI responses with formatted content

## Technologies Used

- **Frontend**: React, TypeScript, TailwindCSS
- **AI Integration**: Google Generative AI (Gemini 1.5 Flash)
- **UI Components**: Custom components with Lucide React icons
- **Build Tools**: Vite, ESLint, PostCSS

## Setup and Installation

### Prerequisites

- Node.js (v18 or newer)
- npm or yarn
- A Google AI Studio API key for Gemini

### Installation Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/ecochoice-ai.git
   cd ecochoice-ai
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   yarn
   ```

3. Create a `.env` file in the root directory with your Gemini API key:
   ```
   VITE_GEMINI_API_KEY=your-api-key-here
   ```

4. Update the API key in the `geminiService.ts` file or use the environment variable:
   ```typescript
   const genAI = new GoogleGenerativeAI(import.meta.env.VITE_GEMINI_API_KEY);
   ```

5. Start the development server:
   ```bash
   npm run dev
   # or
   yarn dev
   ```

6. Open your browser and navigate to `http://localhost:5173`

## Project Structure

- `/src/components` - Reusable UI components
- `/src/pages` - Main page components
- `/src/utils` - Utility functions and services
- `/src/utils/geminiService.ts` - Google Gemini AI integration

## AI Features

The chatbot uses Google's Gemini 1.5 Flash model with custom system instructions to provide:

- Specific product recommendations with example names
- Educational content about sustainability benefits
- Conversational and friendly responses
- Properly formatted output with markdown styling

## Deployment

To build for production:

```bash
npm run build
# or
yarn build
```

The build output will be in the `dist` folder, which can be deployed to any static hosting service like GitHub Pages, Netlify, or Vercel.



## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Google for the Gemini AI API
- Unsplash for the beautiful images
- The React and TailwindCSS communities

---

Created with ❤️ as part of an educational project to promote sustainability through technology.
